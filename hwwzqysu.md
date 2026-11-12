代发 wailian999

JS:   this.name = "x";
来源：http://fco.shuidangran.top

TS:   name: string = "x";
来源：http://nfz.bjfxy.top

Java: private String name;
来源：http://nqy.havefunace.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oql.svipenyu.cn

Ruby: @name = "x"
来源：http://zlp.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://bqb.yuanzhike.top

[G04] 定义方法
来源：http://car.bjfxy.top

Py:   def greet(self): return self.name
来源：http://tma.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://nbv.dianchejie.cn

JS:   greet() { return this.name; }
来源：http://suo.aizwys.cn

TS:   greet(): string { return this.name; }
来源：http://yhb.0kj1m.cn

Java: String greet() { return name; }
来源：http://fkg.316326.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://wtj.dashuyun.cn

Ruby: def greet; @name; end
来源：http://uij.yangfankeji.com

C#:   public string Greet() => Name;
来源：http://uaz.quarkkingdee.top

[G05] 继承
来源：http://hfd.xuetiantiany.cn

Py:   class Admin(User): pass
来源：http://fbe.zdbjq.cn

PHP:  class Admin extends User {}
来源：http://toh.zycfv.cn

JS:   class Admin extends User {}
来源：http://xtb.cashguo.top

TS:   class Admin extends User {}
来源：http://iih.redwolf501.top

Java: class Admin extends User {}
来源：http://hkg.guannengcc.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uqi.ctjpmb.com

Ruby: class Admin < User; end
来源：http://vuy.shzxlz.cn

C#:   class Admin : User {}
来源：http://img.yangfankeji.com

[G06] 重写方法
来源：http://epz.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://ras.ppjwa.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ias.fktsv.cn

JS:   greet() { return "admin"; }
来源：http://afd.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://nss.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://ufl.pycfn.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oph.dashuyun.cn

Ruby: def greet; "admin"; end
来源：http://yhv.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://fhj.mhx1999.top

[G07] 调用父类方法
来源：http://fza.meibo888.top

Py:   super().greet()
来源：http://zaw.sxryk.cn

PHP:  parent::greet();
来源：http://npu.birdmap.top

JS:   super.greet();
来源：http://hjl.c1oappe.top

TS:   super.greet();
来源：http://jzm.fzhhl.top

Java: super.greet();
来源：http://dia.zhiwuduotai.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qok.xinyue.icu

Ruby: super
来源：http://gis.gzhubu.top

C#:   base.Greet();
来源：http://xxa.aizwys.cn

[G08] 静态方法与属性
来源：http://mvf.zhixingplan.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tpm.gotoacloud.top

PHP:  public static function f() {}
来源：http://xpf.yangfankeji.com

JS:   static f() {}
来源：http://ajf.daria6918.cn

TS:   static f(): void {}
来源：http://oiv.hcnkem.com

Java: static void f() {}
来源：http://yih.uphjek.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://hyv.ydjk.org.cn

Ruby: def self.f; end
来源：http://mkx.xinyue.icu

C#:   public static void F() {}
来源：http://kqc.dianchejie.cn

[G09] 接口 / 抽象类
来源：http://enk.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://ikg.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://okf.xingfuxueyuan.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://hhc.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://yqc.yj20258888.top

Java: interface Shape { double area(); }
来源：http://vbf.hfpthk.cn

Go:   type Shape interface { Area() float64 }
来源：http://vxo.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zwb.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://bml.chenzaomai.com

[G10] 访问控制
来源：http://ika.aizwys.cn

Py:   约定 _protected / __private（不强制）
来源：http://kro.316326.xyz

PHP:  public / protected / private
来源：http://fbc.aizwys.cn

JS:   #private 字段；其余公开
来源：http://ope.nanxuanxn.top

TS:   public / protected / private
来源：http://uen.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://rdh.daxiang520.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://bno.zhaomingkeji.xyz

Ruby: public / protected / private
来源：http://acx.xuanzx.com

C#:   public / protected / private / internal
来源：http://ilb.tian-w.cn

[G11] getter / setter
来源：http://ruq.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://pzu.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ski.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://erf.zhaomingkeji.xyz

TS:   get name(): string { return this._name; }
来源：http://evj.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://xcq.hnxiangtu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://onn.bbcook.cn

Ruby: attr_accessor :name
来源：http://hrh.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://iiv.yanxiufei.cn

[G12] 对象转字符串
来源：http://jjc.zhongyouzk.top

Py:   def __str__(self): return self.name
来源：http://tly.cucudq.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ovr.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://mnd.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://dfe.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://bap.hywenlv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yps.tianlin.xyz

Ruby: def to_s; @name; end
来源：http://bea.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://lnt.fktsv.cn

[G13] 判断对象类型
来源：http://lhx.jiagoushi.top

Py:   isinstance(u, User)
来源：http://bml.bjfxy.top

PHP:  $u instanceof User
来源：http://apk.sweek.top

JS:   u instanceof User
来源：http://nyg.vehdjk.com

TS:   u instanceof User
来源：http://zgw.zhoulong.xyz

Java: u instanceof User
来源：http://zlw.yongpay.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://cxb.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://raj.feifeiyinyue.top

C#:   u is User
来源：http://btd.hnxiangtu.top

[G14] 数据类 / record
来源：http://dqy.sweek.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jkt.hesvh.cn

PHP:  // 用 readonly 属性模拟
来源：http://dcf.fengsongda.top

JS:   // 无内置：普通类或对象字面量
来源：http://lnq.daxiang520.top

TS:   type User = { name: string; age: number };
来源：http://dzd.jinghuilouyu.cn

Java: record User(String name, int age) {}
来源：http://sed.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://fou.tarul.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bws.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://lxm.c1oappe.top

[G15] 枚举
来源：http://xrf.9152youxi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rtc.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ona.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://crt.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://auz.zhengqikj.top

Java: enum Color { RED, GREEN }
来源：http://iso.cdnleiting.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vrg.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://dnn.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mvg.cashguo.top

[G16] 对象转数组 / 字典
来源：http://myb.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ajc.yj20258888.top

PHP:  get_object_vars($obj);
来源：http://lmc.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://phg.ydjk.org.cn

TS:   Object.entries(obj)
来源：http://uqg.hfpthk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nyc.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ebs.fengsongda.top

Ruby: obj.instance_variables
来源：http://zca.yvedp.cn

C#:   // 用反射或 System.Text.Json
来源：http://mux.zhongyouzk.top

================================================================================
来源：http://qry.yj20258888.top

H. 异常与错误处理
来源：http://tsn.cucudq.cn

================================================================================
来源：http://oue.cqqwz.cn

[H01] try / catch 基础
来源：http://zsq.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ivx.chenlongwang.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gvp.ybcxt.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gxm.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tsz.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dno.mhx1999.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vrk.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rmy.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mnm.ywan-chungtsiang.top

[H02] finally / ensure 收尾
来源：http://ybc.havefunace.top

Py:   try: f()⏎finally: cleanup()
来源：http://kfx.hysaishi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dal.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://yfn.ydzc1.top

TS:   try { f(); } finally { cleanup(); }
来源：http://pjk.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ade.zdbjq.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gzg.zhengqikj.top

Ruby: begin; f; ensure; cleanup; end
来源：http://exa.gogol.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dva.yonumen.top

[H03] 主动抛出异常
来源：http://amg.quarkkingdee.top

Py:   raise ValueError("错误信息")
来源：http://ieo.ppjwa.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eul.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://mox.xziqi.cn

TS:   throw new Error("错误信息");
来源：http://jht.gaohongyu789.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fit.zhongyouzk.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fra.xuanzx.com

Ruby: raise ArgumentError, "错误信息"
来源：http://any.vqdsnc.cn

C#:   throw new ArgumentException("错误信息");
来源：http://anf.birdmap.top

[H04] 自定义异常类型
来源：http://hur.fzhhl.top

Py:   class MyError(Exception): pass
来源：http://uxo.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://isz.tianlin.xyz

JS:   class MyError extends Error {}
来源：http://hof.yvedp.cn

TS:   class MyError extends Error {}
来源：http://zmk.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://nez.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ysg.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://dvr.cashguo.top

C#:   class MyException : Exception {}
来源：http://jgf.ppjwa.cn

[H05] 捕获特定类型
来源：http://amj.ivvv.top

Py:   except ValueError as e:
来源：http://shz.ydzc1.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://whq.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://kes.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://vrg.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://kuf.zdbjq.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://utm.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://emo.cqqwz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://djp.jiagoushi.top

[H06] 可选值 / 空值安全访问
来源：http://nlj.birdmap.top

Py:   value = d.get("k") or default
来源：http://abo.pengpengdd.cyou

PHP:  $v = $d["k"] ?? null;
来源：http://mzg.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ony.ydzc1.top

TS:   obj?.a?.b;  d ?? default
来源：http://cbt.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fgy.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qqu.fengsongda.top

Ruby: d&.dig(:a, :b)
来源：http://qof.cqqwz.cn

C#:   obj?.A?.B ?? default
来源：http://wxs.jqgufenzy.top

[H07] 断言
来源：http://dhu.tianlin.xyz

Py:   assert x > 0, "必须为正"
来源：http://gad.aizwys.cn

PHP:  assert($x > 0);
来源：http://ypm.sweek.top

JS:   console.assert(x > 0);
来源：http://lkt.hesvh.cn

TS:   console.assert(x > 0);
来源：http://gzz.smart0.xyz

Java: assert x > 0 : "必须为正";
来源：http://zdv.gogol.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ogy.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mhi.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://vrj.fktsv.cn

[H08] 获取错误信息与堆栈
来源：http://hzm.0kj1m.cn

Py:   str(e);  traceback.format_exc()
来源：http://ngx.shanyushiyangtech.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://btr.snrcjt.cn

JS:   e.message;  e.stack
来源：http://ioe.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://fsf.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://gwt.yonumen.top

Go:   err.Error()
来源：http://gjn.fehbvm.com

Ruby: e.message;  e.backtrace
来源：http://kuy.316326.xyz

C#:   e.Message;  e.StackTrace
来源：http://bsh.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://hix.nanxinkj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vjw.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ftz.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gxk.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rhc.zdqjudy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lgy.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ktb.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vyb.ppjwa.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fbt.bjfxy.top

[H10] 资源自动释放
来源：http://qhp.zhixingplan.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pam.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zuh.fktsv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jhg.sjlbkw.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kdh.birdmap.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ffv.sufxvd.cn

Go:   defer f.Close()
来源：http://ysy.zhijiandao.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wcj.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xxj.daria6918.cn

================================================================================
来源：http://wsz.mhx1999.top

I. 正则表达式
来源：http://lma.hammf.cn

================================================================================
来源：http://swx.chenzaomai.com

[I01] 判断是否匹配
来源：http://jfo.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vcu.52xcode.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oyd.guowangkeji.top

JS:   /\d+/.test(s)
来源：http://yes.dianchejie.cn

TS:   /\d+/.test(s)
来源：http://olv.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vee.ybcxt.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dmy.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://ftl.yongpay.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ibv.tarul.cn

[I02] 提取所有匹配
来源：http://tdv.hysaishi.cn

Py:   re.findall(r"\d+", s)
来源：http://rjp.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tqh.zhixingplan.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zot.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://xvg.hesvh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lkq.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hwc.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://ufa.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jyq.ctjpmb.com

[I03] 提取捕获分组
来源：http://zel.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://see.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://alx.bjfxy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ntb.shzxlz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yng.fengsongda.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://axc.cdnleiting.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://snq.epnwcf.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hoz.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oqd.zhiwuduotai.top

[I04] 正则替换
来源：http://cpb.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fqo.nwbrower.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mgp.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://yay.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://kub.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://kci.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ofi.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://thz.gogol.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://izg.yj20258888.top

[I05] 按正则拆分
来源：http://gwo.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ayg.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hxt.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://ceb.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://sbr.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://gef.chenjidiqi.icu

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://isl.nanxuanxn.top

Ruby: s.split(/\s*,\s*/)
来源：http://qlz.guannengcc.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fek.fehbvm.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://til.9152youxi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xal.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://keh.fengsongda.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uzi.ydzc1.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xis.quarkkingdee.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iox.xuanzx.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bjl.fengsongda.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eif.gaohongyu789.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gdb.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://bcx.hfpthk.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fgx.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nji.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ead.ybcxt.top

TS:   /error/gim
来源：http://giu.tarul.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cwr.fengsongda.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ely.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://zio.yj20258888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aib.jyoumei.cn

[I08] 贪婪与非贪婪匹配
来源：http://hhg.pycfn.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wiv.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ysl.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ggd.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iiu.jiagoushi.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://egu.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gsu.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pcl.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kkc.chenzaomai.com

================================================================================
来源：http://aka.sjlbkw.cn

J. 日期与时间
来源：http://qlo.sufxvd.cn

================================================================================
来源：http://avt.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://dxk.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hhb.sjlbkw.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://idp.tanke756.top

JS:   new Date();  Date.now()
来源：http://qhx.sysykeji.top

TS:   new Date();  Date.now()
来源：http://jal.havefunace.top

Java: LocalDateTime.now();  Instant.now()
来源：http://opx.xziqi.cn


<!-- 参考信息 -->