代发 wailian999

[G02] 构造函数
来源：http://sio.tarul.cn

Py:   def __init__(self, name): self.name = name
来源：http://ufj.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://skp.sysykeji.top

JS:   constructor(name) { this.name = name; }
来源：http://uaz.jlsjyb.cn

TS:   constructor(public name: string) {}
来源：http://arj.gaohongyu789.top

Java: User(String name) { this.name = name; }
来源：http://duz.yuxming.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iaq.zdbjq.cn

Ruby: def initialize(name); @name = name; end
来源：http://xea.wangdashe.top

C#:   public User(string name) { Name = name; }
来源：http://maj.52xcode.cn

[G03] 实例属性
来源：http://ghw.yj202588.top

Py:   self.name = "x"
来源：http://ozh.fanxiaobao.xyz

PHP:  public string $name = "x";
来源：http://kzs.jinqigfzy.top

JS:   this.name = "x";
来源：http://pyu.jiagoushi.top

TS:   name: string = "x";
来源：http://pyw.shanyushiyangtech.top

Java: private String name;
来源：http://lel.gogol.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blv.zhixingplan.top

Ruby: @name = "x"
来源：http://biv.kuanghao11.cn

C#:   public string Name { get; set; } = "x";
来源：http://jdg.pycfn.com

[G04] 定义方法
来源：http://yau.zdbjq.cn

Py:   def greet(self): return self.name
来源：http://rjp.jinghuilouyu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tdj.jianghu66.top

JS:   greet() { return this.name; }
来源：http://fhe.havefunace.top

TS:   greet(): string { return this.name; }
来源：http://ylm.sjlbkw.cn

Java: String greet() { return name; }
来源：http://pke.jiagoushi.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://uzq.jlsjyb.cn

Ruby: def greet; @name; end
来源：http://urg.ybcxt.top

C#:   public string Greet() => Name;
来源：http://kdx.zhoulong.xyz

[G05] 继承
来源：http://ljr.yj20258.top

Py:   class Admin(User): pass
来源：http://oxx.ydjk.org.cn

PHP:  class Admin extends User {}
来源：http://zej.ydjk.org.cn

JS:   class Admin extends User {}
来源：http://dpd.sweek.top

TS:   class Admin extends User {}
来源：http://rtm.tarul.cn

Java: class Admin extends User {}
来源：http://dju.0kj1m.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gfo.cucudq.cn

Ruby: class Admin < User; end
来源：http://rvl.jinyuanbaomall.cn

C#:   class Admin : User {}
来源：http://zsz.gzhubu.top

[G06] 重写方法
来源：http://ypw.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://vti.52xcode.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://afi.hcnkem.com

JS:   greet() { return "admin"; }
来源：http://bcn.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://dxd.shzxlz.cn

Java: @Override String greet() { return "admin"; }
来源：http://dpk.ehwqpu.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qhx.jinqigufen.top

Ruby: def greet; "admin"; end
来源：http://znv.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://reo.gogol.net.cn

[G07] 调用父类方法
来源：http://cke.andypj.xyz

Py:   super().greet()
来源：http://kti.cheryme.top

PHP:  parent::greet();
来源：http://ezc.jqgufenzy.top

JS:   super.greet();
来源：http://hqc.gogol.net.cn

TS:   super.greet();
来源：http://phw.ctjpmb.com

Java: super.greet();
来源：http://ean.9152youxi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jtj.birdmap.top

Ruby: super
来源：http://voh.hywenlv.cn

C#:   base.Greet();
来源：http://dbs.shangyingyoupin.top

[G08] 静态方法与属性
来源：http://qje.xziqi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rgy.xinyue.icu

PHP:  public static function f() {}
来源：http://bot.hywenlv.cn

JS:   static f() {}
来源：http://nhh.cqqwz.cn

TS:   static f(): void {}
来源：http://xzo.quarkkingdee.top

Java: static void f() {}
来源：http://xap.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://gyf.yangfankeji.com

Ruby: def self.f; end
来源：http://xul.chenlongwang.top

C#:   public static void F() {}
来源：http://iew.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://uuh.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://nyv.shzxlz.cn

PHP:  interface Shape { public function area(): float; }
来源：http://esq.yj20258.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://iwy.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://cvs.haohaochexian.top

Java: interface Shape { double area(); }
来源：http://ysu.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://ise.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://itr.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://hfs.fzhhl.top

[G10] 访问控制
来源：http://mfo.yonumen.top

Py:   约定 _protected / __private（不强制）
来源：http://asv.ctjpmb.com

PHP:  public / protected / private
来源：http://zoh.chenjidiqi.icu

JS:   #private 字段；其余公开
来源：http://num.redwolf501.top

TS:   public / protected / private
来源：http://upv.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://raa.zhiwuduotai.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kdf.chenlongwang.top

Ruby: public / protected / private
来源：http://rhp.yanxiufei.cn

C#:   public / protected / private / internal
来源：http://ceg.aizwys.cn

[G11] getter / setter
来源：http://coa.chenlongwang.top

Py:   @property 与 @x.setter
来源：http://moy.jinqigufen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://bbd.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://plt.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://tld.uphjek.com

Java: public String getName() { return name; }
来源：http://ssw.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://zjq.kuanghao11.cn

Ruby: attr_accessor :name
来源：http://utx.zhijiandao.cn

C#:   public string Name { get; set; }
来源：http://fga.cqqwz.cn

[G12] 对象转字符串
来源：http://tbk.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://epl.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://ead.sweek.top

JS:   toString() { return this.name; }
来源：http://gvz.zycfv.cn

TS:   toString(): string { return this.name; }
来源：http://uds.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://wob.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://igq.zdqjudy.top

Ruby: def to_s; @name; end
来源：http://mvk.birdmap.top

C#:   public override string ToString() => Name;
来源：http://wwa.uphjek.com

[G13] 判断对象类型
来源：http://lyw.fehbvm.com

Py:   isinstance(u, User)
来源：http://gid.epnwcf.com

PHP:  $u instanceof User
来源：http://msm.yuxming.cn

JS:   u instanceof User
来源：http://qvj.cucudq.cn

TS:   u instanceof User
来源：http://oor.hnxiangtu.top

Java: u instanceof User
来源：http://afk.jianghu66.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lzt.aizwys.cn

Ruby: u.is_a?(User)
来源：http://zzi.daria6918.cn

C#:   u is User
来源：http://zgr.fzhhl.top

[G14] 数据类 / record
来源：http://fxz.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fxh.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://kfj.fktsv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://aix.tanke756.top

TS:   type User = { name: string; age: number };
来源：http://mms.nwbrower.top

Java: record User(String name, int age) {}
来源：http://eyf.gogol.net.cn

Go:   type User struct { Name string; Age int }
来源：http://wsy.gzhubu.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mmi.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://wgc.yfazqb.com

[G15] 枚举
来源：http://ohn.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://umw.tianlin.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://zkh.yanxiufei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yoq.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://flq.zhiwuduotai.top

Java: enum Color { RED, GREEN }
来源：http://gdz.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qay.kuanghao11.cn

Ruby: Color = %i[red green].freeze
来源：http://lem.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kyd.cheryme.top

[G16] 对象转数组 / 字典
来源：http://utk.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yio.wangdashe.top

PHP:  get_object_vars($obj);
来源：http://szs.hesvh.cn

JS:   Object.entries(obj)
来源：http://uby.yanxiufei.cn

TS:   Object.entries(obj)
来源：http://zlg.xuanzx.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://psi.ppjwa.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cky.ctjpmb.com

Ruby: obj.instance_variables
来源：http://nev.tianlin.xyz

C#:   // 用反射或 System.Text.Json
来源：http://qjc.hfpthk.cn

================================================================================
来源：http://zrh.hnqzz.top

H. 异常与错误处理
来源：http://ijy.ydzc1.top

================================================================================
来源：http://aql.bjfxy.top

[H01] try / catch 基础
来源：http://xbm.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rkd.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://upg.ydjk.org.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dtb.zdbjq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gud.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zey.feifeiyinyue.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kij.yuxming.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dfl.zdqjudy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zth.jinghuilouyu.cn

[H02] finally / ensure 收尾
来源：http://uuj.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://yvo.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://aok.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://qhj.hnqzz.top

TS:   try { f(); } finally { cleanup(); }
来源：http://vdk.meibo888.top

Java: try { f(); } finally { cleanup(); }
来源：http://qbq.yonumen.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dkh.uphjek.com

Ruby: begin; f; ensure; cleanup; end
来源：http://cxe.redwolf501.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://huz.ivvv.top

[H03] 主动抛出异常
来源：http://hmx.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://lfc.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vhk.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://ljs.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://bbm.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfq.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dnd.nwbrower.top

Ruby: raise ArgumentError, "错误信息"
来源：http://irn.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://ohb.hcnkem.com

[H04] 自定义异常类型
来源：http://bmp.kuanghao11.cn

Py:   class MyError(Exception): pass
来源：http://blz.tanke756.top

PHP:  class MyError extends RuntimeException {}
来源：http://cat.ybcxt.top

JS:   class MyError extends Error {}
来源：http://ynm.meibo888.top

TS:   class MyError extends Error {}
来源：http://biw.hesvh.cn

Java: class MyException extends RuntimeException {}
来源：http://ery.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rjc.yfazqb.com

Ruby: class MyError < StandardError; end
来源：http://saj.yanxiufei.cn

C#:   class MyException : Exception {}
来源：http://jyh.shanyushiyangkeji.top

[H05] 捕获特定类型
来源：http://fbh.hesvh.cn

Py:   except ValueError as e:
来源：http://jkt.jqgufenzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sjo.shanyushiyangtech.top

JS:   if (e instanceof TypeError) {}
来源：http://ikl.chenjidiqi.icu

TS:   if (e instanceof TypeError) {}
来源：http://drt.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://qdz.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://skt.yongpay.top

Ruby: rescue ArgumentError => e
来源：http://ptw.tarul.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mhp.c1oappe.top

[H06] 可选值 / 空值安全访问
来源：http://car.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://lix.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://uhe.zhoulong.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://yxd.hnqzz.top

TS:   obj?.a?.b;  d ?? default
来源：http://rpe.chenjidiqi.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bry.bbcook.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wvc.fzhhl.top

Ruby: d&.dig(:a, :b)
来源：http://kgz.nanxinkj.top

C#:   obj?.A?.B ?? default
来源：http://ngg.fanxiaobao.xyz

[H07] 断言
来源：http://nee.0kj1m.cn

Py:   assert x > 0, "必须为正"
来源：http://woe.bjfxy.top

PHP:  assert($x > 0);
来源：http://byb.fzhhl.top

JS:   console.assert(x > 0);
来源：http://zbm.gotoacloud.top

TS:   console.assert(x > 0);
来源：http://ryk.zhiwuduotai.top

Java: assert x > 0 : "必须为正";
来源：http://vki.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jgq.tanke756.top

Ruby: raise "必须为正" unless x > 0
来源：http://wro.guannengcc.top

C#:   Debug.Assert(x > 0);
来源：http://anc.gogol.net.cn

[H08] 获取错误信息与堆栈
来源：http://bto.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://drq.yvedp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jkj.fehbvm.com

JS:   e.message;  e.stack
来源：http://crj.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://evv.xylfe.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qdq.tanke756.top

Go:   err.Error()
来源：http://pcg.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://hnx.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://lnq.zhoulong.xyz

[H09] 带错误码的异常
来源：http://blb.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pfl.bbcook.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vat.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mna.zhiwuduotai.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qcl.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zxo.gogol.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oxd.sysykeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://ecm.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rfe.jianghu66.top

[H10] 资源自动释放
来源：http://ihm.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hpj.fanxiaobao.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jon.hongshengwenyu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lzv.havefunace.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vso.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tqn.hesvh.cn

Go:   defer f.Close()
来源：http://cub.shanyushiyangtech.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jsw.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dsu.yongpay.top

================================================================================
来源：http://rrf.jinyuanbaomall.cn

I. 正则表达式
来源：http://muw.dianchejie.cn

================================================================================
来源：http://nrr.cucudq.cn

[I01] 判断是否匹配
来源：http://pyp.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pem.jyoumei.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yck.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://hgq.xingfuxueyuan.xyz

TS:   /\d+/.test(s)
来源：http://ped.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xbf.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kka.feifeiyinyue.top

Ruby: s.match?(/\d+/)
来源：http://nfz.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vze.redwolf501.top

[I02] 提取所有匹配
来源：http://wih.yj202588.top

Py:   re.findall(r"\d+", s)
来源：http://tco.cqqwz.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ldi.iojbl.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kar.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://qdx.gogol.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nmi.ivvv.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ibj.hongshengwenyu.top

Ruby: s.scan(/\d+/)
来源：http://xdp.ctjpmb.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vxu.gogol.net.cn

[I03] 提取捕获分组
来源：http://bfw.cashguo.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wqc.jianghu66.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://knf.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uop.sufxvd.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cwo.cqqwz.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hdo.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jeb.hnxiangtu.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gqz.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tpd.hywenlv.cn

[I04] 正则替换
来源：http://zrp.andypj.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jtl.hywenlv.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dil.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://xru.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://waf.jinqigufen.top

Java: s.replaceAll("\\d+", "#")
来源：http://rni.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jer.fehbvm.com

Ruby: s.gsub(/\d+/, "#")
来源：http://ikp.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iht.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://rsn.zhaomingkeji.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://sml.shanyushiyangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ueh.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://ekk.meibo888.top

TS:   s.split(/\s*,\s*/)
来源：http://bgi.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://lwp.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://aww.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gbt.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bbi.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lis.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jyc.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cet.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cwr.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsc.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mzm.jinghuilouyu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://upg.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cuu.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rir.ctjpmb.com

[I07] 忽略大小写与多行模式
来源：http://aud.zycfv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dmz.gogol.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qii.yj20258.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qzs.yfazqb.com

TS:   /error/gim
来源：http://zgt.epnwcf.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qjt.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qrx.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://ptf.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kpc.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://yze.52xcode.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kyp.zhiwuduotai.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jma.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xvg.dashuyun.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fym.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lwe.hywenlv.cn


<!-- 参考信息 -->