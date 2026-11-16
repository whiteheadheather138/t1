代发 wailian999

TS:   constructor(public name: string) {}
来源：http://yvy.shanyushiyangkeji.top

Java: User(String name) { this.name = name; }
来源：http://vqw.ctjpmb.com

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://njt.aizwys.cn

Ruby: def initialize(name); @name = name; end
来源：http://qqr.pycfn.com

C#:   public User(string name) { Name = name; }
来源：http://ftt.shangyingyoupin.top

[G03] 实例属性
来源：http://uhs.wangdashe.top

Py:   self.name = "x"
来源：http://wxm.yongpay.top

PHP:  public string $name = "x";
来源：http://cvo.gaohongyu789.top

JS:   this.name = "x";
来源：http://lyo.gotoacloud.top

TS:   name: string = "x";
来源：http://jdr.yj20258.top

Java: private String name;
来源：http://kus.yanxiufei.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yys.xylfe.cn

Ruby: @name = "x"
来源：http://ifc.vqdsnc.cn

C#:   public string Name { get; set; } = "x";
来源：http://tzf.chenjidiqi.icu

[G04] 定义方法
来源：http://pfk.hesvh.cn

Py:   def greet(self): return self.name
来源：http://ory.daxiang520.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qnt.tarul.cn

JS:   greet() { return this.name; }
来源：http://tyc.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://zij.dianchejie.cn

Java: String greet() { return name; }
来源：http://kma.yvedp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ori.zdbjq.cn

Ruby: def greet; @name; end
来源：http://cct.vqdsnc.cn

C#:   public string Greet() => Name;
来源：http://asb.yuanzhike.top

[G05] 继承
来源：http://wbu.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://qxi.kuanghao11.cn

PHP:  class Admin extends User {}
来源：http://ozc.zhengqikj.top

JS:   class Admin extends User {}
来源：http://pax.meibo888.top

TS:   class Admin extends User {}
来源：http://hcq.316326.xyz

Java: class Admin extends User {}
来源：http://alg.quarkkingdee.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uqo.sjlbkw.cn

Ruby: class Admin < User; end
来源：http://drh.jinqigufen.top

C#:   class Admin : User {}
来源：http://crj.zdbjq.cn

[G06] 重写方法
来源：http://vgs.yj20258888.top

Py:   def greet(self): return "admin"
来源：http://idj.0kj1m.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dwr.gotoacloud.top

JS:   greet() { return "admin"; }
来源：http://jnw.c1oappe.top

TS:   greet(): string { return "admin"; }
来源：http://rrn.guannengcc.top

Java: @Override String greet() { return "admin"; }
来源：http://zou.iojbl.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://anu.aizwys.cn

Ruby: def greet; "admin"; end
来源：http://cvn.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://zkk.daria6918.cn

[G07] 调用父类方法
来源：http://ytz.hcnkem.com

Py:   super().greet()
来源：http://mvj.snrcjt.cn

PHP:  parent::greet();
来源：http://xzb.chenjidiqi.icu

JS:   super.greet();
来源：http://vqo.fehbvm.com

TS:   super.greet();
来源：http://uvv.zhiwuduotai.top

Java: super.greet();
来源：http://uys.havefunace.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xbn.mhx1999.top

Ruby: super
来源：http://cra.zhijiandao.cn

C#:   base.Greet();
来源：http://kal.chenlongwang.top

[G08] 静态方法与属性
来源：http://hfo.0kj1m.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uro.hywenlv.cn

PHP:  public static function f() {}
来源：http://udq.xylfe.cn

JS:   static f() {}
来源：http://zsw.tianlin.xyz

TS:   static f(): void {}
来源：http://lht.gzhubu.top

Java: static void f() {}
来源：http://yhd.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://utj.dianchejie.cn

Ruby: def self.f; end
来源：http://itj.jinqigfzy.top

C#:   public static void F() {}
来源：http://ofd.zhaomingkeji.xyz

[G09] 接口 / 抽象类
来源：http://pzw.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://hzk.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://oxp.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://tix.fehbvm.com

TS:   interface Shape { area(): number; }
来源：http://gez.nanxinkj.top

Java: interface Shape { double area(); }
来源：http://zge.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://hmy.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wsl.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://won.chenlongwang.top

[G10] 访问控制
来源：http://yar.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://pnx.fehbvm.com

PHP:  public / protected / private
来源：http://rml.yangfankeji.com

JS:   #private 字段；其余公开
来源：http://myw.shanyushiyangtech.top

TS:   public / protected / private
来源：http://xfb.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://gmp.ydjk.org.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://muv.shzxlz.cn

Ruby: public / protected / private
来源：http://vhs.gogol.net.cn

C#:   public / protected / private / internal
来源：http://lfh.andypj.xyz

[G11] getter / setter
来源：http://miv.zhongyouzk.top

Py:   @property 与 @x.setter
来源：http://zwq.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jhl.fengsongda.top

JS:   get name() { return this._name; }
来源：http://oop.andypj.xyz

TS:   get name(): string { return this._name; }
来源：http://plc.chenjidiqi.icu

Java: public String getName() { return name; }
来源：http://uuf.iojbl.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mws.gotoacloud.top

Ruby: attr_accessor :name
来源：http://zqw.ybcxt.top

C#:   public string Name { get; set; }
来源：http://dol.cqqwz.cn

[G12] 对象转字符串
来源：http://edo.xinyue.icu

Py:   def __str__(self): return self.name
来源：http://qvp.jiagoushi.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://acj.yuxming.cn

JS:   toString() { return this.name; }
来源：http://ozy.redwolf501.top

TS:   toString(): string { return this.name; }
来源：http://dzq.yongpay.top

Java: @Override public String toString() { return name; }
来源：http://aej.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gpe.ivvv.top

Ruby: def to_s; @name; end
来源：http://sip.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://rcn.zdbjq.cn

[G13] 判断对象类型
来源：http://sbr.wangdashe.top

Py:   isinstance(u, User)
来源：http://qbz.ybcxt.top

PHP:  $u instanceof User
来源：http://fou.snrcjt.cn

JS:   u instanceof User
来源：http://guq.cheryme.top

TS:   u instanceof User
来源：http://smc.guowangkeji.top

Java: u instanceof User
来源：http://zdv.chenlongwang.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://uuy.haohaochexian.top

Ruby: u.is_a?(User)
来源：http://zip.daxiang520.top

C#:   u is User
来源：http://iwe.ppjwa.cn

[G14] 数据类 / record
来源：http://ijt.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pfn.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://ezu.c1oappe.top

JS:   // 无内置：普通类或对象字面量
来源：http://fid.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://zjm.pycfn.com

Java: record User(String name, int age) {}
来源：http://ags.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://ygv.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rkm.haohaochexian.top

C#:   record User(string Name, int Age);
来源：http://skz.hfpthk.cn

[G15] 枚举
来源：http://bmn.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zfm.daria6918.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pil.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ydh.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eeb.zycfv.cn

Java: enum Color { RED, GREEN }
来源：http://vrt.xinyue.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zjt.jqgufenzy.top

Ruby: Color = %i[red green].freeze
来源：http://hmg.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://evp.hfpthk.cn

[G16] 对象转数组 / 字典
来源：http://cca.nanxuanxn.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xsq.shuidangran.top

PHP:  get_object_vars($obj);
来源：http://mrt.aibaodan.cn

JS:   Object.entries(obj)
来源：http://ijn.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://sds.gaohongyu789.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dth.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://wia.0kj1m.cn

Ruby: obj.instance_variables
来源：http://fws.nanxinkj.top

C#:   // 用反射或 System.Text.Json
来源：http://cgk.hnqzz.top

================================================================================
来源：http://ycp.zhoulong.xyz

H. 异常与错误处理
来源：http://wqv.tanke756.top

================================================================================
来源：http://gqc.jlsjyb.cn

[H01] try / catch 基础
来源：http://yyo.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iis.iojbl.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://idz.nwbrower.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gnr.sufxvd.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kvw.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mez.hfpthk.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kuj.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vqk.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vqe.vehdjk.com

[H02] finally / ensure 收尾
来源：http://kln.nwbrower.top

Py:   try: f()⏎finally: cleanup()
来源：http://kyr.hfpthk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jiv.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hey.yj20258.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hrp.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://pvt.guowangkeji.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://fvi.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://wkb.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wtp.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://wlt.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://jvh.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bkm.zycfv.cn

JS:   throw new Error("错误信息");
来源：http://fys.pycfn.com

TS:   throw new Error("错误信息");
来源：http://nsp.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lbo.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dsd.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mvo.gogol.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://egq.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://mwf.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://slx.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://snu.yuxming.cn

JS:   class MyError extends Error {}
来源：http://zyq.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://eje.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://qob.zhoulong.xyz

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ipg.zhoulong.xyz

Ruby: class MyError < StandardError; end
来源：http://ftu.tarul.cn

C#:   class MyException : Exception {}
来源：http://igt.tian-w.cn

[H05] 捕获特定类型
来源：http://tzo.gogol.net.cn

Py:   except ValueError as e:
来源：http://fdh.shzxlz.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kzy.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://gbo.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://rka.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://tci.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mhn.hnxiangtu.top

Ruby: rescue ArgumentError => e
来源：http://odq.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://znm.tarul.cn

[H06] 可选值 / 空值安全访问
来源：http://kxc.9152youxi.cn

Py:   value = d.get("k") or default
来源：http://aau.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://drd.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://jdo.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uvk.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cif.snrcjt.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ecc.52xcode.cn

Ruby: d&.dig(:a, :b)
来源：http://vul.zhaomingkeji.xyz

C#:   obj?.A?.B ?? default
来源：http://huk.c1oappe.top

[H07] 断言
来源：http://pfe.yuxming.cn

Py:   assert x > 0, "必须为正"
来源：http://tyn.iojbl.cn

PHP:  assert($x > 0);
来源：http://jvw.meibo888.top

JS:   console.assert(x > 0);
来源：http://ssd.jianghu66.top

TS:   console.assert(x > 0);
来源：http://xdq.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://vuq.bbcook.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bug.jianghu66.top

Ruby: raise "必须为正" unless x > 0
来源：http://tys.chenjidiqi.icu

C#:   Debug.Assert(x > 0);
来源：http://yeh.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://pvd.daxiang520.top

Py:   str(e);  traceback.format_exc()
来源：http://kuf.cheryme.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zml.chenjidiqi.icu

JS:   e.message;  e.stack
来源：http://lyo.vqdsnc.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ppo.ydzc1.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cte.sufxvd.cn

Go:   err.Error()
来源：http://epz.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://cac.jiagoushi.top

C#:   e.Message;  e.StackTrace
来源：http://pyi.vqdsnc.cn

[H09] 带错误码的异常
来源：http://jid.zdbjq.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zlj.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://exv.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zws.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://csd.shanyushiyangtech.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nrl.jianghu66.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://btl.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://dzv.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://luq.zhongyouzk.top

[H10] 资源自动释放
来源：http://ueb.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wrn.yj20258888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kfu.jqgfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xsk.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hfo.yj20258888.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ibg.fktsv.cn

Go:   defer f.Close()
来源：http://upn.shangyingyoupin.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cqp.shuidangran.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cpy.hongshengwenyu.top

================================================================================
来源：http://hhe.nanxuanxn.top

I. 正则表达式
来源：http://bib.cqqwz.cn

================================================================================
来源：http://qdv.nwbrower.top

[I01] 判断是否匹配
来源：http://kfo.kuanghao11.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://drt.shanyushiyangkeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://jjs.pycfn.com

JS:   /\d+/.test(s)
来源：http://icx.yj20258.top

TS:   /\d+/.test(s)
来源：http://toj.yonumen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gzk.sxryk.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://huj.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://oiv.tian-w.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dun.hysaishi.cn

[I02] 提取所有匹配
来源：http://xti.cheryme.top

Py:   re.findall(r"\d+", s)
来源：http://ndp.c1oappe.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iqs.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ssg.sjlbkw.cn

TS:   s.match(/\d+/g)
来源：http://hgk.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vya.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dzh.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://qwn.hnqzz.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lwn.hysaishi.cn

[I03] 提取捕获分组
来源：http://jue.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tkr.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fvb.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xcq.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uxy.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oou.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pra.ehwqpu.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hub.mhx1999.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ycd.wangshuangyany.cn

[I04] 正则替换
来源：http://ynz.zhongyouzk.top

Py:   re.sub(r"\d+", "#", s)
来源：http://utn.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mcr.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://hmz.shanyushiyangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://vsk.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://yxt.fanxiaobao.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://aeq.nanxuanxn.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dix.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://doz.haohaochexian.top

[I05] 按正则拆分
来源：http://zjh.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ytj.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iqq.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://mqk.haohaochexian.top

TS:   s.split(/\s*,\s*/)
来源：http://aaz.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://rqu.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://woc.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://txg.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oma.sufxvd.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lvy.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wes.ywan-chungtsiang.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ilk.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uhi.hcnkem.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mkp.zhaomingkeji.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ppo.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xyp.zdqjudy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gyv.cdnleiting.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dty.yuxming.cn

[I07] 忽略大小写与多行模式
来源：http://tti.xinyue.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bsb.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ngm.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zll.havefunace.top

TS:   /error/gim
来源：http://cbw.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zpq.cqqwz.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hbp.sweek.top

Ruby: s.scan(/error/i)
来源：http://nkl.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pgd.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://wdx.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iob.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://afe.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://trt.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tmk.xingfuxueyuan.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://lnh.xingfuxueyuan.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kjr.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zmt.tarul.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kwa.hcnkem.com

================================================================================
来源：http://wgq.jiagoushi.top


<!-- 参考信息 -->