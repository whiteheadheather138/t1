代发 wailian999

JS:   this.name = "x";
来源：http://jra.yanxiufei.cn

TS:   name: string = "x";
来源：http://qdj.fehbvm.com

Java: private String name;
来源：http://rch.xziqi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://smd.fehbvm.com

Ruby: @name = "x"
来源：http://nxg.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://irm.mhx1999.top

[G04] 定义方法
来源：http://udq.yuanzhike.top

Py:   def greet(self): return self.name
来源：http://oap.xinyue.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://uzj.daxiang520.top

JS:   greet() { return this.name; }
来源：http://mnx.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://nyr.sysykeji.top

Java: String greet() { return name; }
来源：http://chx.hesvh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://umu.xziqi.cn

Ruby: def greet; @name; end
来源：http://fyl.pengpengdd.cyou

C#:   public string Greet() => Name;
来源：http://kqh.xingfuxueyuan.xyz

[G05] 继承
来源：http://opf.pengpengdd.cyou

Py:   class Admin(User): pass
来源：http://tsy.redwolf501.top

PHP:  class Admin extends User {}
来源：http://xua.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://xtm.dianchejie.cn

TS:   class Admin extends User {}
来源：http://iar.jianghu66.top

Java: class Admin extends User {}
来源：http://vix.sweek.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kkl.tanke756.top

Ruby: class Admin < User; end
来源：http://kgv.hnqzz.top

C#:   class Admin : User {}
来源：http://vtp.jinqigfzy.top

[G06] 重写方法
来源：http://bpf.zdbjq.cn

Py:   def greet(self): return "admin"
来源：http://urn.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xdt.chenjidiqi.icu

JS:   greet() { return "admin"; }
来源：http://fvh.gaohongyu789.top

TS:   greet(): string { return "admin"; }
来源：http://kya.andypj.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ukx.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fxc.shzxlz.cn

Ruby: def greet; "admin"; end
来源：http://msu.nwbrower.top

C#:   public override string Greet() => "admin";
来源：http://qjb.zycfv.cn

[G07] 调用父类方法
来源：http://roh.fktsv.cn

Py:   super().greet()
来源：http://epr.hesvh.cn

PHP:  parent::greet();
来源：http://fko.hnxiangtu.top

JS:   super.greet();
来源：http://dpg.0kj1m.cn

TS:   super.greet();
来源：http://xqg.zhoulong.xyz

Java: super.greet();
来源：http://dlm.tarul.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gml.xuanzx.com

Ruby: super
来源：http://loi.xylfe.cn

C#:   base.Greet();
来源：http://xgg.andypj.xyz

[G08] 静态方法与属性
来源：http://oig.vehdjk.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uhc.zhijiandao.cn

PHP:  public static function f() {}
来源：http://xcm.tian-w.cn

JS:   static f() {}
来源：http://hjy.bjfxy.top

TS:   static f(): void {}
来源：http://cby.smart0.xyz

Java: static void f() {}
来源：http://buo.jinghuilouyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hgm.gzhubu.top

Ruby: def self.f; end
来源：http://aet.jinqigfzy.top

C#:   public static void F() {}
来源：http://mdh.zdqjudy.top

[G09] 接口 / 抽象类
来源：http://pus.ctjpmb.com

Py:   from abc import ABC, abstractmethod
来源：http://pjs.gaohongyu789.top

PHP:  interface Shape { public function area(): float; }
来源：http://imn.ehwqpu.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ekr.ctjpmb.com

TS:   interface Shape { area(): number; }
来源：http://pww.tian-w.cn

Java: interface Shape { double area(); }
来源：http://vyr.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://gmr.chenzaomai.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dkg.meibo888.top

C#:   interface IShape { double Area(); }
来源：http://hwf.yfazqb.com

[G10] 访问控制
来源：http://kce.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://vqv.yj20258.top

PHP:  public / protected / private
来源：http://smd.ppjwa.cn

JS:   #private 字段；其余公开
来源：http://wup.hysaishi.cn

TS:   public / protected / private
来源：http://jtb.vehdjk.com

Java: public / protected / private / 默认包级
来源：http://lwg.gzhubu.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://sfv.fktsv.cn

Ruby: public / protected / private
来源：http://ffb.epnwcf.com

C#:   public / protected / private / internal
来源：http://ijr.tianlin.xyz

[G11] getter / setter
来源：http://oyq.jqgfzy.top

Py:   @property 与 @x.setter
来源：http://fgy.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://lrj.xziqi.cn

JS:   get name() { return this._name; }
来源：http://toc.jiagoushi.top

TS:   get name(): string { return this._name; }
来源：http://iaz.aizwys.cn

Java: public String getName() { return name; }
来源：http://tpu.ivvv.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://gdl.tarul.cn

Ruby: attr_accessor :name
来源：http://qdm.cheryme.top

C#:   public string Name { get; set; }
来源：http://eul.xziqi.cn

[G12] 对象转字符串
来源：http://irf.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://tds.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xvw.sweek.top

JS:   toString() { return this.name; }
来源：http://afy.cqqwz.cn

TS:   toString(): string { return this.name; }
来源：http://emy.fanxiaobao.xyz

Java: @Override public String toString() { return name; }
来源：http://tmj.shzxlz.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wnc.tarul.cn

Ruby: def to_s; @name; end
来源：http://szy.sjlbkw.cn

C#:   public override string ToString() => Name;
来源：http://ecn.hongshengwenyu.top

[G13] 判断对象类型
来源：http://gij.hongshengwenyu.top

Py:   isinstance(u, User)
来源：http://mft.zhoulong.xyz

PHP:  $u instanceof User
来源：http://kva.ydzc1.top

JS:   u instanceof User
来源：http://daw.sweek.top

TS:   u instanceof User
来源：http://mdi.9152youxi.cn

Java: u instanceof User
来源：http://iyt.tanke756.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://bru.cheryme.top

Ruby: u.is_a?(User)
来源：http://afx.ydjk.org.cn

C#:   u is User
来源：http://vzl.kuanghao11.cn

[G14] 数据类 / record
来源：http://igh.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ifb.yuanzhike.top

PHP:  // 用 readonly 属性模拟
来源：http://peq.pycfn.com

JS:   // 无内置：普通类或对象字面量
来源：http://ona.zhoulong.xyz

TS:   type User = { name: string; age: number };
来源：http://zbq.nanxinkj.top

Java: record User(String name, int age) {}
来源：http://uyf.bjfxy.top

Go:   type User struct { Name string; Age int }
来源：http://vcx.cqqwz.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hhl.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://fie.xuanzx.com

[G15] 枚举
来源：http://ybw.gotoacloud.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gli.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yqt.jqgfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://spe.zhiwuduotai.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hxq.snrcjt.cn

Java: enum Color { RED, GREEN }
来源：http://gni.316326.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vol.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://wci.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xaa.bjfxy.top

[G16] 对象转数组 / 字典
来源：http://vjk.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rkk.yueranfly.top

PHP:  get_object_vars($obj);
来源：http://lhf.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://xsh.kuanghao11.cn

TS:   Object.entries(obj)
来源：http://bnb.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ikk.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vtx.epnwcf.com

Ruby: obj.instance_variables
来源：http://gdf.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://ijl.jianghu66.top

================================================================================
来源：http://ovm.chenlongwang.top

H. 异常与错误处理
来源：http://qla.meibo888.top

================================================================================
来源：http://rtn.zdqjudy.top

[H01] try / catch 基础
来源：http://dbx.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yjr.xuetiantiany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jin.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zix.gotoacloud.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fzy.wangdashe.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oby.chenlongwang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hli.yj20258888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://axi.tarul.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://apf.52xcode.cn

[H02] finally / ensure 收尾
来源：http://elz.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://syb.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://oyr.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ajy.shanyushiyangkeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kfr.sweek.top

Java: try { f(); } finally { cleanup(); }
来源：http://tuu.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fep.yj20258888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://yzw.uphjek.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://pti.vqdsnc.cn

[H03] 主动抛出异常
来源：http://sks.sufxvd.cn

Py:   raise ValueError("错误信息")
来源：http://zoo.xuanzx.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fwh.sxryk.cn

JS:   throw new Error("错误信息");
来源：http://pqn.pengpengdd.cyou

TS:   throw new Error("错误信息");
来源：http://vwc.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://psq.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cbj.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://aba.zycfv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ysl.fengsongda.top

[H04] 自定义异常类型
来源：http://bmw.cashguo.top

Py:   class MyError(Exception): pass
来源：http://oay.jiagoushi.top

PHP:  class MyError extends RuntimeException {}
来源：http://beu.aizwys.cn

JS:   class MyError extends Error {}
来源：http://mly.zhiwuduotai.top

TS:   class MyError extends Error {}
来源：http://azj.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://dbl.jyoumei.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wle.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://cll.fktsv.cn

C#:   class MyException : Exception {}
来源：http://dqt.yanxiufei.cn

[H05] 捕获特定类型
来源：http://nyq.yanxiufei.cn

Py:   except ValueError as e:
来源：http://dkl.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://irc.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://ntp.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://bhv.sxryk.cn

Java: catch (IOException | SQLException e) {}
来源：http://lmt.hysaishi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dxe.zdqjudy.top

Ruby: rescue ArgumentError => e
来源：http://zoy.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jxt.yuanzhike.top

[H06] 可选值 / 空值安全访问
来源：http://wji.jiagoushi.top

Py:   value = d.get("k") or default
来源：http://cwj.nwbrower.top

PHP:  $v = $d["k"] ?? null;
来源：http://qfs.fengsongda.top

JS:   obj?.a?.b;  d ?? default
来源：http://cdk.zdqjudy.top

TS:   obj?.a?.b;  d ?? default
来源：http://kwl.jinyuanbaomall.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nuk.jinqigfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uyz.daria6918.cn

Ruby: d&.dig(:a, :b)
来源：http://zxn.shzxlz.cn

C#:   obj?.A?.B ?? default
来源：http://qwe.chenjidiqi.icu

[H07] 断言
来源：http://mgk.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://njj.hnxiangtu.top

PHP:  assert($x > 0);
来源：http://nvl.yuxming.cn

JS:   console.assert(x > 0);
来源：http://pzi.dashuyun.cn

TS:   console.assert(x > 0);
来源：http://abh.ppjwa.cn

Java: assert x > 0 : "必须为正";
来源：http://mcc.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dya.feifeiyinyue.top

Ruby: raise "必须为正" unless x > 0
来源：http://ltu.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://acl.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://nnd.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://qow.ivvv.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gld.yfazqb.com

JS:   e.message;  e.stack
来源：http://ucm.hcnkem.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://ddd.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ikt.hysaishi.cn

Go:   err.Error()
来源：http://ztm.zhongyouzk.top

Ruby: e.message;  e.backtrace
来源：http://ikj.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://mzi.yj202588.top

[H09] 带错误码的异常
来源：http://lno.uphjek.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xbe.xziqi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wnk.jinyuanbaomall.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dny.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iwt.dianchejie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dwr.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ccp.tian-w.cn

Ruby: raise MyError.new("fail", 500)
来源：http://onx.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://eoh.aibaodan.cn

[H10] 资源自动释放
来源：http://brn.fzhhl.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cxq.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ejq.guannengcc.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bmi.epnwcf.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ysj.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xyy.cashguo.top

Go:   defer f.Close()
来源：http://htb.tianlin.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wwa.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qkp.jlsjyb.cn

================================================================================
来源：http://pwo.cucudq.cn

I. 正则表达式
来源：http://ogk.redwolf501.top

================================================================================
来源：http://jek.ydzc1.top

[I01] 判断是否匹配
来源：http://abr.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ijl.hammf.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dpc.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://fte.0kj1m.cn

TS:   /\d+/.test(s)
来源：http://irm.ywan-chungtsiang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lvg.yvedp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wwu.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://tgi.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tjj.ehwqpu.com

[I02] 提取所有匹配
来源：http://ilk.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://ssl.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xgu.kuanghao11.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mdr.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://aja.jqgfzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vhu.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tgp.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://ddx.0kj1m.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bum.sufxvd.cn

[I03] 提取捕获分组
来源：http://tmk.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jyk.guowangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://djf.svipenyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fvn.daxiang520.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kex.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jth.zhixingplan.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://joz.aizwys.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wph.hysaishi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ahk.iojbl.cn

[I04] 正则替换
来源：http://obd.pengpengdd.cyou

Py:   re.sub(r"\d+", "#", s)
来源：http://upi.havefunace.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xqn.redwolf501.top

JS:   s.replace(/\d+/g, "#")
来源：http://eze.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zcm.guowangkeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://vfw.zdqjudy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cwy.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://qce.zhongyouzk.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mzc.hnxiangtu.top

[I05] 按正则拆分
来源：http://pet.cheryme.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dnc.jinqigfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ujl.pycfn.com

JS:   s.split(/\s*,\s*/)
来源：http://ndu.smart0.xyz

TS:   s.split(/\s*,\s*/)
来源：http://mzl.dashuyun.cn

Java: s.split("\\s*,\\s*")
来源：http://xkw.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://akr.cdnleiting.top

Ruby: s.split(/\s*,\s*/)
来源：http://yoi.quarkkingdee.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ggq.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yvj.shuidangran.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://smg.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ois.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nzz.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ups.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://juz.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jjy.ivvv.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xaa.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://weq.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://xex.zhixingplan.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fui.daxiang520.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qzl.sxryk.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://syl.yongpay.top

TS:   /error/gim
来源：http://ytr.hfpthk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dwx.gzhubu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://how.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://fff.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wdh.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://amv.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eaq.quarkkingdee.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bqw.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bzy.snrcjt.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ati.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cwd.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gbg.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mwt.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uzl.yvedp.cn

================================================================================
来源：http://pfs.gzhubu.top

J. 日期与时间
来源：http://tci.aizwys.cn

================================================================================
来源：http://gqw.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://bpg.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://lto.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xcm.ydzc1.top

JS:   new Date();  Date.now()
来源：http://icr.yj202588.top

TS:   new Date();  Date.now()
来源：http://qgv.vehdjk.com

Java: LocalDateTime.now();  Instant.now()
来源：http://qzt.jianghu66.top


<!-- 参考信息 -->