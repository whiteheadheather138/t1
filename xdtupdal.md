代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qjs.yueranfly.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ofe.pengpengdd.cyou

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gfx.yanxiufei.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wyf.daria6918.cn

================================================================================
来源：http://svz.redwolf501.top

G. 面向对象
来源：http://fur.birdmap.top

================================================================================
来源：http://ddb.yangfankeji.com

[G01] 定义类
来源：http://plr.hysaishi.cn

Py:   class User: pass
来源：http://qsz.yonumen.top

PHP:  class User {}
来源：http://far.yuxming.cn

JS:   class User {}
来源：http://ywd.jqgfzy.top

TS:   class User { name: string = ""; }
来源：http://wef.52xcode.cn

Java: class User {}
来源：http://fvz.wangshuangyany.cn

Go:   type User struct { Name string }
来源：http://hyt.ydzc1.top

Ruby: class User; end
来源：http://yat.haohaochexian.top

C#:   class User {}
来源：http://hoi.feifeiyinyue.top

[G02] 构造函数
来源：http://jvj.havefunace.top

Py:   def __init__(self, name): self.name = name
来源：http://uxc.jinghuilouyu.cn

PHP:  public function __construct(public string $name) {}
来源：http://sky.cheryme.top

JS:   constructor(name) { this.name = name; }
来源：http://oac.tianlin.xyz

TS:   constructor(public name: string) {}
来源：http://urs.daria6918.cn

Java: User(String name) { this.name = name; }
来源：http://yie.feifeiyinyue.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yim.jyoumei.cn

Ruby: def initialize(name); @name = name; end
来源：http://qsb.jqgfzy.top

C#:   public User(string name) { Name = name; }
来源：http://bxd.smart0.xyz

[G03] 实例属性
来源：http://rof.tarul.cn

Py:   self.name = "x"
来源：http://deh.yongpay.top

PHP:  public string $name = "x";
来源：http://pdr.tian-w.cn

JS:   this.name = "x";
来源：http://ngt.sjlbkw.cn

TS:   name: string = "x";
来源：http://cby.gaohongyu789.top

Java: private String name;
来源：http://lsz.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bso.yuxming.cn

Ruby: @name = "x"
来源：http://tiu.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://psw.havefunace.top

[G04] 定义方法
来源：http://spi.bjfxy.top

Py:   def greet(self): return self.name
来源：http://wfa.shanyushiyangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tcf.chenlongwang.top

JS:   greet() { return this.name; }
来源：http://ute.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://kso.aibaodan.cn

Java: String greet() { return name; }
来源：http://xfu.kuanghao11.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hxt.chenlongwang.top

Ruby: def greet; @name; end
来源：http://hbr.andypj.xyz

C#:   public string Greet() => Name;
来源：http://kss.ydzc1.top

[G05] 继承
来源：http://lpq.guannengcc.top

Py:   class Admin(User): pass
来源：http://nez.andypj.xyz

PHP:  class Admin extends User {}
来源：http://ilp.shuidangran.top

JS:   class Admin extends User {}
来源：http://qvw.cdnleiting.top

TS:   class Admin extends User {}
来源：http://rzm.yuxming.cn

Java: class Admin extends User {}
来源：http://oez.yuxming.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://txb.ppjwa.cn

Ruby: class Admin < User; end
来源：http://lda.bjfxy.top

C#:   class Admin : User {}
来源：http://dkh.xingfuxueyuan.xyz

[G06] 重写方法
来源：http://vnq.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://fil.chenjidiqi.icu

PHP:  public function greet(): string { return "admin"; }
来源：http://llp.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://ynr.bbcook.cn

TS:   greet(): string { return "admin"; }
来源：http://eio.zhoulong.xyz

Java: @Override String greet() { return "admin"; }
来源：http://lun.hnxiangtu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rcu.mhx1999.top

Ruby: def greet; "admin"; end
来源：http://kwq.fengsongda.top

C#:   public override string Greet() => "admin";
来源：http://uvd.jqgufenzy.top

[G07] 调用父类方法
来源：http://edx.havefunace.top

Py:   super().greet()
来源：http://xeb.ybcxt.top

PHP:  parent::greet();
来源：http://xco.birdmap.top

JS:   super.greet();
来源：http://nyx.fzhhl.top

TS:   super.greet();
来源：http://uvd.tianlin.xyz

Java: super.greet();
来源：http://hza.nanxuanxn.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dgo.nanxinkj.top

Ruby: super
来源：http://xzg.yvedp.cn

C#:   base.Greet();
来源：http://kcj.meibo888.top

[G08] 静态方法与属性
来源：http://dvr.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zlm.chenlongwang.top

PHP:  public static function f() {}
来源：http://gqb.chenzaomai.com

JS:   static f() {}
来源：http://qcp.yj20258.top

TS:   static f(): void {}
来源：http://nua.shzxlz.cn

Java: static void f() {}
来源：http://axh.dianchejie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mdx.yfazqb.com

Ruby: def self.f; end
来源：http://orq.mhx1999.top

C#:   public static void F() {}
来源：http://hrl.fehbvm.com

[G09] 接口 / 抽象类
来源：http://oqp.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://vuq.nwbrower.top

PHP:  interface Shape { public function area(): float; }
来源：http://axe.yanxiufei.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bla.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://vfq.zhixingplan.top

Java: interface Shape { double area(); }
来源：http://feh.kuanghao11.cn

Go:   type Shape interface { Area() float64 }
来源：http://klv.hywenlv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rye.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://xaj.tian-w.cn

[G10] 访问控制
来源：http://fdz.xziqi.cn

Py:   约定 _protected / __private（不强制）
来源：http://olg.bjfxy.top

PHP:  public / protected / private
来源：http://hsb.redwolf501.top

JS:   #private 字段；其余公开
来源：http://vvh.sweek.top

TS:   public / protected / private
来源：http://cvu.jinghuilouyu.cn

Java: public / protected / private / 默认包级
来源：http://cea.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xkx.cqqwz.cn

Ruby: public / protected / private
来源：http://dej.hnqzz.top

C#:   public / protected / private / internal
来源：http://rlf.pycfn.com

[G11] getter / setter
来源：http://mab.bjfxy.top

Py:   @property 与 @x.setter
来源：http://pdw.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eci.zhiwuduotai.top

JS:   get name() { return this._name; }
来源：http://itq.ywan-chungtsiang.top

TS:   get name(): string { return this._name; }
来源：http://rhc.aizwys.cn

Java: public String getName() { return name; }
来源：http://kjj.ywan-chungtsiang.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://anj.yangfankeji.com

Ruby: attr_accessor :name
来源：http://jno.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://mmu.jlsjyb.cn

[G12] 对象转字符串
来源：http://mrs.quarkkingdee.top

Py:   def __str__(self): return self.name
来源：http://ece.shangyingyoupin.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://fcf.c1oappe.top

JS:   toString() { return this.name; }
来源：http://puk.daria6918.cn

TS:   toString(): string { return this.name; }
来源：http://woq.vehdjk.com

Java: @Override public String toString() { return name; }
来源：http://hmo.jinghuilouyu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dww.yfazqb.com

Ruby: def to_s; @name; end
来源：http://mbb.nanxuanxn.top

C#:   public override string ToString() => Name;
来源：http://lje.jqgufenzy.top

[G13] 判断对象类型
来源：http://blf.uphjek.com

Py:   isinstance(u, User)
来源：http://mjd.fehbvm.com

PHP:  $u instanceof User
来源：http://mcj.yj20258.top

JS:   u instanceof User
来源：http://dif.nwbrower.top

TS:   u instanceof User
来源：http://ivy.hcnkem.com

Java: u instanceof User
来源：http://gtq.hnqzz.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://yge.ctjpmb.com

Ruby: u.is_a?(User)
来源：http://pwz.xingfuxueyuan.xyz

C#:   u is User
来源：http://jmy.cheryme.top

[G14] 数据类 / record
来源：http://acf.mhx1999.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zkg.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://tuw.shangyingyoupin.top

JS:   // 无内置：普通类或对象字面量
来源：http://dcy.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://jxz.cashguo.top

Java: record User(String name, int age) {}
来源：http://yxi.tarul.cn

Go:   type User struct { Name string; Age int }
来源：http://vlr.vehdjk.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mer.yonumen.top

C#:   record User(string Name, int Age);
来源：http://tyz.kuanghao11.cn

[G15] 枚举
来源：http://ean.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://twa.aizwys.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oxu.jianghu66.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lvl.yj202588.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dva.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://trg.hesvh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kal.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://gsl.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://doo.jqgufenzy.top

[G16] 对象转数组 / 字典
来源：http://prm.tanke756.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rbg.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://fnl.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://cnp.c1oappe.top

TS:   Object.entries(obj)
来源：http://nml.jiagoushi.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zbd.dianchejie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qwg.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://vbp.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://wls.zdbjq.cn

================================================================================
来源：http://zfy.gaohongyu789.top

H. 异常与错误处理
来源：http://gwf.haohaochexian.top

================================================================================
来源：http://wdc.hnqzz.top

[H01] try / catch 基础
来源：http://gqw.yangfankeji.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://anb.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rdy.zdbjq.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jkv.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://coq.tarul.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://luk.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yyf.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wpu.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://als.sxryk.cn

[H02] finally / ensure 收尾
来源：http://qfb.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://asb.yj20258888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://etx.snrcjt.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mwi.quarkkingdee.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rce.chenjidiqi.icu

Java: try { f(); } finally { cleanup(); }
来源：http://oqs.jinqigufen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://agz.xuanzx.com

Ruby: begin; f; ensure; cleanup; end
来源：http://svs.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://srx.tian-w.cn

[H03] 主动抛出异常
来源：http://obb.birdmap.top

Py:   raise ValueError("错误信息")
来源：http://smo.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mgh.c1oappe.top

JS:   throw new Error("错误信息");
来源：http://dil.jianghu66.top

TS:   throw new Error("错误信息");
来源：http://jyy.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kca.zhengqikj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qpz.yuanzhike.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ijk.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://vxl.vqdsnc.cn

[H04] 自定义异常类型
来源：http://xkn.ydzc1.top

Py:   class MyError(Exception): pass
来源：http://uul.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jas.hcnkem.com

JS:   class MyError extends Error {}
来源：http://lul.andypj.xyz

TS:   class MyError extends Error {}
来源：http://aay.hcnkem.com

Java: class MyException extends RuntimeException {}
来源：http://ffy.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jto.hywenlv.cn

Ruby: class MyError < StandardError; end
来源：http://sqx.zhiwuduotai.top

C#:   class MyException : Exception {}
来源：http://emd.hysaishi.cn

[H05] 捕获特定类型
来源：http://otr.redwolf501.top

Py:   except ValueError as e:
来源：http://wmz.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aqu.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://tzo.cdnleiting.top

TS:   if (e instanceof TypeError) {}
来源：http://ceb.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://rfo.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qvi.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://iva.shuidangran.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fte.hongshengwenyu.top

[H06] 可选值 / 空值安全访问
来源：http://gvn.sxryk.cn

Py:   value = d.get("k") or default
来源：http://ook.jinyuanbaomall.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jgr.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://qxo.andypj.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://lku.tanke756.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qwl.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jmg.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://pnx.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://fxw.yj202588.top

[H07] 断言
来源：http://bsy.yueranfly.top

Py:   assert x > 0, "必须为正"
来源：http://ihw.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://qpg.meibo888.top

JS:   console.assert(x > 0);
来源：http://sya.sweek.top

TS:   console.assert(x > 0);
来源：http://osb.feifeiyinyue.top

Java: assert x > 0 : "必须为正";
来源：http://fri.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pfr.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mix.gogol.net.cn

C#:   Debug.Assert(x > 0);
来源：http://yml.sweek.top

[H08] 获取错误信息与堆栈
来源：http://gdy.nanxinkj.top

Py:   str(e);  traceback.format_exc()
来源：http://dan.jinqigfzy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bvf.9152youxi.cn

JS:   e.message;  e.stack
来源：http://kei.wangshuangyany.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fsl.hnqzz.top

Java: e.getMessage();  e.printStackTrace()
来源：http://pym.birdmap.top

Go:   err.Error()
来源：http://rcw.jianghu66.top

Ruby: e.message;  e.backtrace
来源：http://fkv.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://omn.fzhhl.top

[H09] 带错误码的异常
来源：http://duq.ybcxt.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ufs.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://aau.zhixingplan.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jrw.vehdjk.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iss.yongpay.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ceb.guannengcc.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://psy.shanyushiyangtech.top

Ruby: raise MyError.new("fail", 500)
来源：http://obs.andypj.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://hai.zhixingplan.top

[H10] 资源自动释放
来源：http://vch.gzhubu.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hby.nanxinkj.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wir.jiagoushi.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dlk.shanyushiyangtech.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://chi.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ezs.epnwcf.com

Go:   defer f.Close()
来源：http://uoc.jyoumei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bpr.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uhz.nanxinkj.top

================================================================================
来源：http://axm.zdqjudy.top

I. 正则表达式
来源：http://xpm.9152youxi.cn

================================================================================
来源：http://gmj.fzhhl.top

[I01] 判断是否匹配
来源：http://hkw.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qpt.guowangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://vmc.vehdjk.com

JS:   /\d+/.test(s)
来源：http://hhn.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://roe.c1oappe.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mxa.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ogf.jlsjyb.cn

Ruby: s.match?(/\d+/)
来源：http://gte.guannengcc.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zbf.hnqzz.top

[I02] 提取所有匹配
来源：http://nfg.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://gzw.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lbe.yonumen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ida.316326.xyz

TS:   s.match(/\d+/g)
来源：http://mso.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://onz.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ltx.uphjek.com

Ruby: s.scan(/\d+/)
来源：http://hqi.meibo888.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qzl.daxiang520.top

[I03] 提取捕获分组
来源：http://kvz.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ixp.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pcs.smart0.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xav.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rgp.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wmn.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hnp.shanyushiyangkeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zin.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jhl.nanxinkj.top

[I04] 正则替换
来源：http://xda.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wei.hcnkem.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zpj.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://zik.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fpt.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fvv.9152youxi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://unv.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mog.sufxvd.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cnb.nanxuanxn.top

[I05] 按正则拆分
来源：http://xda.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rcj.jyoumei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ptw.xylfe.cn

JS:   s.split(/\s*,\s*/)
来源：http://qeo.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://gej.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://szs.zhiwuduotai.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://enj.hcnkem.com

Ruby: s.split(/\s*,\s*/)
来源：http://qcn.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://chs.ehwqpu.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mnz.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lof.hammf.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tcz.zhongyouzk.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oln.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wfo.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uii.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ksq.gaohongyu789.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://keq.cashguo.top


<!-- 参考信息 -->