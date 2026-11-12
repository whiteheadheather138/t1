代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hmt.52xcode.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pqk.tanke756.top

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nrz.xingfuxueyuan.xyz

TS:   // 同上
来源：http://yzw.hammf.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gxd.chenlongwang.top

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vep.jinqigfzy.top

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jux.tian-w.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vuo.bbcook.cn

================================================================================
来源：http://zkd.xziqi.cn

G. 面向对象
来源：http://njh.cqqwz.cn

================================================================================
来源：http://hxh.wangshuangyany.cn

[G01] 定义类
来源：http://wut.jinyuanbaomall.cn

Py:   class User: pass
来源：http://blb.yvedp.cn

PHP:  class User {}
来源：http://suk.fzhhl.top

JS:   class User {}
来源：http://ezj.meibo888.top

TS:   class User { name: string = ""; }
来源：http://maw.daxiang520.top

Java: class User {}
来源：http://mob.haohaochexian.top

Go:   type User struct { Name string }
来源：http://jzn.cashguo.top

Ruby: class User; end
来源：http://nez.shuidangran.top

C#:   class User {}
来源：http://thn.hnqzz.top

[G02] 构造函数
来源：http://lkx.guannengcc.top

Py:   def __init__(self, name): self.name = name
来源：http://dvq.uphjek.com

PHP:  public function __construct(public string $name) {}
来源：http://tvb.c1oappe.top

JS:   constructor(name) { this.name = name; }
来源：http://ooj.jianghu66.top

TS:   constructor(public name: string) {}
来源：http://xoc.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://hxx.hysaishi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lha.shangyingyoupin.top

Ruby: def initialize(name); @name = name; end
来源：http://btc.hcnkem.com

C#:   public User(string name) { Name = name; }
来源：http://vvu.dianchejie.cn

[G03] 实例属性
来源：http://fzp.smart0.xyz

Py:   self.name = "x"
来源：http://csj.daxiang520.top

PHP:  public string $name = "x";
来源：http://rkv.52xcode.cn

JS:   this.name = "x";
来源：http://wka.yj20258888.top

TS:   name: string = "x";
来源：http://vca.daria6918.cn

Java: private String name;
来源：http://vjs.gzhubu.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jwl.bbcook.cn

Ruby: @name = "x"
来源：http://qpy.fzhhl.top

C#:   public string Name { get; set; } = "x";
来源：http://mhd.jinghuilouyu.cn

[G04] 定义方法
来源：http://jaw.fehbvm.com

Py:   def greet(self): return self.name
来源：http://jid.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cvw.hywenlv.cn

JS:   greet() { return this.name; }
来源：http://nyj.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://rbr.shzxlz.cn

Java: String greet() { return name; }
来源：http://npd.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lta.birdmap.top

Ruby: def greet; @name; end
来源：http://org.zycfv.cn

C#:   public string Greet() => Name;
来源：http://smg.andypj.xyz

[G05] 继承
来源：http://gtc.havefunace.top

Py:   class Admin(User): pass
来源：http://cbp.zhiwuduotai.top

PHP:  class Admin extends User {}
来源：http://trq.iojbl.cn

JS:   class Admin extends User {}
来源：http://zfj.redwolf501.top

TS:   class Admin extends User {}
来源：http://toh.yfazqb.com

Java: class Admin extends User {}
来源：http://ndj.meibo888.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hdx.nanxinkj.top

Ruby: class Admin < User; end
来源：http://tua.cashguo.top

C#:   class Admin : User {}
来源：http://diw.aizwys.cn

[G06] 重写方法
来源：http://tdc.zhoulong.xyz

Py:   def greet(self): return "admin"
来源：http://scb.guannengcc.top

PHP:  public function greet(): string { return "admin"; }
来源：http://ppr.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://nav.cdnleiting.top

TS:   greet(): string { return "admin"; }
来源：http://aee.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://pjy.shuidangran.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://skk.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://hva.316326.xyz

C#:   public override string Greet() => "admin";
来源：http://mpc.ppjwa.cn

[G07] 调用父类方法
来源：http://sor.nwbrower.top

Py:   super().greet()
来源：http://pxu.guowangkeji.top

PHP:  parent::greet();
来源：http://fui.zhengqikj.top

JS:   super.greet();
来源：http://vin.ivvv.top

TS:   super.greet();
来源：http://dmu.zycfv.cn

Java: super.greet();
来源：http://bup.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cgw.yongpay.top

Ruby: super
来源：http://don.smart0.xyz

C#:   base.Greet();
来源：http://lxj.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://pyo.hnqzz.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hbh.yj20258888.top

PHP:  public static function f() {}
来源：http://kvl.316326.xyz

JS:   static f() {}
来源：http://jil.hnqzz.top

TS:   static f(): void {}
来源：http://ndd.cdnleiting.top

Java: static void f() {}
来源：http://wrb.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wda.jqgufenzy.top

Ruby: def self.f; end
来源：http://mks.shanyushiyangkeji.top

C#:   public static void F() {}
来源：http://wbz.hywenlv.cn

[G09] 接口 / 抽象类
来源：http://dsx.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://myu.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://hap.guowangkeji.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zod.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://mjv.smart0.xyz

Java: interface Shape { double area(); }
来源：http://cym.zhijiandao.cn

Go:   type Shape interface { Area() float64 }
来源：http://nhu.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ttk.guowangkeji.top

C#:   interface IShape { double Area(); }
来源：http://euu.cheryme.top

[G10] 访问控制
来源：http://ict.hnqzz.top

Py:   约定 _protected / __private（不强制）
来源：http://del.hnqzz.top

PHP:  public / protected / private
来源：http://aor.fengsongda.top

JS:   #private 字段；其余公开
来源：http://qtq.kuanghao11.cn

TS:   public / protected / private
来源：http://cvc.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://rjc.jqgfzy.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vjg.aizwys.cn

Ruby: public / protected / private
来源：http://dlv.tian-w.cn

C#:   public / protected / private / internal
来源：http://vnt.zhengqikj.top

[G11] getter / setter
来源：http://atw.uphjek.com

Py:   @property 与 @x.setter
来源：http://bax.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://fov.xylfe.cn

JS:   get name() { return this._name; }
来源：http://lfg.kuanghao11.cn

TS:   get name(): string { return this._name; }
来源：http://ajm.yuxming.cn

Java: public String getName() { return name; }
来源：http://grc.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cav.gzhubu.top

Ruby: attr_accessor :name
来源：http://hbu.yj20258888.top

C#:   public string Name { get; set; }
来源：http://mxt.quarkkingdee.top

[G12] 对象转字符串
来源：http://ryy.jlsjyb.cn

Py:   def __str__(self): return self.name
来源：http://jxi.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dpf.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://sfh.fengsongda.top

TS:   toString(): string { return this.name; }
来源：http://zct.shanyushiyangkeji.top

Java: @Override public String toString() { return name; }
来源：http://xed.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://jef.nwbrower.top

Ruby: def to_s; @name; end
来源：http://dca.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://jcd.yuanzhike.top

[G13] 判断对象类型
来源：http://wtn.xylfe.cn

Py:   isinstance(u, User)
来源：http://isz.yvedp.cn

PHP:  $u instanceof User
来源：http://uay.jinghuilouyu.cn

JS:   u instanceof User
来源：http://oyt.hywenlv.cn

TS:   u instanceof User
来源：http://qvt.hywenlv.cn

Java: u instanceof User
来源：http://ijt.jinqigfzy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ruw.ybcxt.top

Ruby: u.is_a?(User)
来源：http://fym.daxiang520.top

C#:   u is User
来源：http://bog.ydjk.org.cn

[G14] 数据类 / record
来源：http://xgc.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fod.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://cqf.jyoumei.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pjc.hammf.cn

TS:   type User = { name: string; age: number };
来源：http://nzs.hcnkem.com

Java: record User(String name, int age) {}
来源：http://abp.hesvh.cn

Go:   type User struct { Name string; Age int }
来源：http://crv.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mhh.cashguo.top

C#:   record User(string Name, int Age);
来源：http://pvo.yj202588.top

[G15] 枚举
来源：http://jei.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aub.hnqzz.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://yzg.aizwys.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zgg.jianghu66.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ytu.zdqjudy.top

Java: enum Color { RED, GREEN }
来源：http://wsj.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yeu.shanyushiyangtech.top

Ruby: Color = %i[red green].freeze
来源：http://pdr.guowangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xbt.hywenlv.cn

[G16] 对象转数组 / 字典
来源：http://lra.xziqi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aqf.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://tmz.jyoumei.cn

JS:   Object.entries(obj)
来源：http://bhn.epnwcf.com

TS:   Object.entries(obj)
来源：http://skc.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zko.fengsongda.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lcd.zdqjudy.top

Ruby: obj.instance_variables
来源：http://fsh.shangyingyoupin.top

C#:   // 用反射或 System.Text.Json
来源：http://nez.jinghuilouyu.cn

================================================================================
来源：http://tqy.uphjek.com

H. 异常与错误处理
来源：http://xet.yuanzhike.top

================================================================================
来源：http://ggm.xuanzx.com

[H01] try / catch 基础
来源：http://qdk.ydjk.org.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aaj.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://smk.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bkv.aizwys.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kdo.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bpp.bjfxy.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jgj.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sfu.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://snx.haohaochexian.top

[H02] finally / ensure 收尾
来源：http://qlz.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pya.daxiang520.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://prg.haohaochexian.top

JS:   try { f(); } finally { cleanup(); }
来源：http://izd.tarul.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pab.jqgufenzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://blb.sysykeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zub.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://lqg.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hld.svipenyu.cn

[H03] 主动抛出异常
来源：http://zpc.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://wlv.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wpu.yonumen.top

JS:   throw new Error("错误信息");
来源：http://chb.hnqzz.top

TS:   throw new Error("错误信息");
来源：http://hat.cucudq.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bvk.fehbvm.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xpq.jinqigufen.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fbg.ydzc1.top

C#:   throw new ArgumentException("错误信息");
来源：http://xop.xuetiantiany.cn

[H04] 自定义异常类型
来源：http://cts.yuanzhike.top

Py:   class MyError(Exception): pass
来源：http://phu.tarul.cn

PHP:  class MyError extends RuntimeException {}
来源：http://puk.sjlbkw.cn

JS:   class MyError extends Error {}
来源：http://dfw.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://ghu.jqgfzy.top

Java: class MyException extends RuntimeException {}
来源：http://qqz.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uxt.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://ndo.c1oappe.top

C#:   class MyException : Exception {}
来源：http://hte.yuanzhike.top

[H05] 捕获特定类型
来源：http://iiy.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://gfx.jinghuilouyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rgs.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://dxt.yfazqb.com

TS:   if (e instanceof TypeError) {}
来源：http://iyv.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://dyy.cucudq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hax.nanxinkj.top

Ruby: rescue ArgumentError => e
来源：http://kei.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://piu.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://cae.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://ojz.tarul.cn

PHP:  $v = $d["k"] ?? null;
来源：http://leh.shanyushiyangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://apu.jinqigfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://trq.jlsjyb.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bwp.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hbd.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://uls.quarkkingdee.top

C#:   obj?.A?.B ?? default
来源：http://ffv.hcnkem.com

[H07] 断言
来源：http://fbx.jianghu66.top

Py:   assert x > 0, "必须为正"
来源：http://pnd.ehwqpu.com

PHP:  assert($x > 0);
来源：http://ygt.fehbvm.com

JS:   console.assert(x > 0);
来源：http://xfv.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://yrq.zhaomingkeji.xyz

Java: assert x > 0 : "必须为正";
来源：http://efj.tarul.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jre.ppjwa.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cye.birdmap.top

C#:   Debug.Assert(x > 0);
来源：http://bvc.tianlin.xyz

[H08] 获取错误信息与堆栈
来源：http://lan.yj20258888.top

Py:   str(e);  traceback.format_exc()
来源：http://hkx.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lxv.sxryk.cn

JS:   e.message;  e.stack
来源：http://gkf.nwbrower.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qoi.ehwqpu.com

Java: e.getMessage();  e.printStackTrace()
来源：http://yck.uphjek.com

Go:   err.Error()
来源：http://gdk.meibo888.top

Ruby: e.message;  e.backtrace
来源：http://xlh.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://qrw.hammf.cn

[H09] 带错误码的异常
来源：http://snp.nanxuanxn.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bey.jinghuilouyu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tae.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fdq.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ska.nanxuanxn.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://trx.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://syg.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://qlh.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://vzg.fanxiaobao.xyz

[H10] 资源自动释放
来源：http://rtf.zhengqikj.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cfr.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ths.xuanzx.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ncc.haohaochexian.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zwu.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zeu.pengpengdd.cyou

Go:   defer f.Close()
来源：http://cng.zhiwuduotai.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ahw.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qoc.havefunace.top

================================================================================
来源：http://zjf.xuetiantiany.cn

I. 正则表达式
来源：http://owo.hnxiangtu.top

================================================================================
来源：http://dsj.daria6918.cn

[I01] 判断是否匹配
来源：http://ddw.zhijiandao.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ran.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://guj.316326.xyz

JS:   /\d+/.test(s)
来源：http://yxd.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://ihl.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://udj.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nmu.chenzaomai.com

Ruby: s.match?(/\d+/)
来源：http://vsx.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ahu.jinqigfzy.top

[I02] 提取所有匹配
来源：http://uju.bjfxy.top

Py:   re.findall(r"\d+", s)
来源：http://srl.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oul.yongpay.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nce.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://vtq.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mmj.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xow.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://jrp.zycfv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://khm.sweek.top

[I03] 提取捕获分组
来源：http://jki.yanxiufei.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xln.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xfw.shanyushiyangtech.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ikz.jqgfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kzo.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gzx.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://buv.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vbd.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://msf.hammf.cn

[I04] 正则替换
来源：http://qpl.nwbrower.top

Py:   re.sub(r"\d+", "#", s)
来源：http://icc.hesvh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zfo.cashguo.top

JS:   s.replace(/\d+/g, "#")
来源：http://kff.xingfuxueyuan.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://hrn.52xcode.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ofa.aibaodan.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hun.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://tgw.xuanzx.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://awv.nwbrower.top

[I05] 按正则拆分
来源：http://slk.svipenyu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nan.316326.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gqy.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://uib.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://nyc.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://nrj.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nkb.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pki.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rmi.yfazqb.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lsq.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vdc.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wyu.guannengcc.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://twr.yfazqb.com


<!-- 参考信息 -->