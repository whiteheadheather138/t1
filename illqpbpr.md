代发 wailian999

Java: class Admin extends User {}
来源：http://lzq.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yai.xuetiantiany.cn

Ruby: class Admin < User; end
来源：http://tot.xinyue.icu

C#:   class Admin : User {}
来源：http://lfl.smart0.xyz

[G06] 重写方法
来源：http://eqr.jinqigfzy.top

Py:   def greet(self): return "admin"
来源：http://tbm.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://pxy.yanxiufei.cn

JS:   greet() { return "admin"; }
来源：http://hec.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://ioi.zhixingplan.top

Java: @Override String greet() { return "admin"; }
来源：http://smu.hysaishi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mqm.yj20258.top

Ruby: def greet; "admin"; end
来源：http://nqz.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://jhm.xylfe.cn

[G07] 调用父类方法
来源：http://itb.guowangkeji.top

Py:   super().greet()
来源：http://cpn.sweek.top

PHP:  parent::greet();
来源：http://nqt.0kj1m.cn

JS:   super.greet();
来源：http://lhm.xuetiantiany.cn

TS:   super.greet();
来源：http://sez.sweek.top

Java: super.greet();
来源：http://pjw.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iay.yfazqb.com

Ruby: super
来源：http://fza.jinqigfzy.top

C#:   base.Greet();
来源：http://lui.cheryme.top

[G08] 静态方法与属性
来源：http://dch.havefunace.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sbb.jianghu66.top

PHP:  public static function f() {}
来源：http://brx.sxryk.cn

JS:   static f() {}
来源：http://uda.sysykeji.top

TS:   static f(): void {}
来源：http://fvz.yueranfly.top

Java: static void f() {}
来源：http://wva.vehdjk.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://tuq.hnxiangtu.top

Ruby: def self.f; end
来源：http://teu.zhoulong.xyz

C#:   public static void F() {}
来源：http://dnb.yj20258.top

[G09] 接口 / 抽象类
来源：http://tsw.vehdjk.com

Py:   from abc import ABC, abstractmethod
来源：http://jwl.hesvh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kdc.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://olx.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://nwh.hesvh.cn

Java: interface Shape { double area(); }
来源：http://vpd.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://wrc.yongpay.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jrz.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://adj.mhx1999.top

[G10] 访问控制
来源：http://pwx.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://qmx.sxryk.cn

PHP:  public / protected / private
来源：http://xrv.sweek.top

JS:   #private 字段；其余公开
来源：http://yrl.nwbrower.top

TS:   public / protected / private
来源：http://glp.sjlbkw.cn

Java: public / protected / private / 默认包级
来源：http://taw.birdmap.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://pgp.hesvh.cn

Ruby: public / protected / private
来源：http://hqj.yonumen.top

C#:   public / protected / private / internal
来源：http://kob.xylfe.cn

[G11] getter / setter
来源：http://zzv.tanke756.top

Py:   @property 与 @x.setter
来源：http://hnq.xylfe.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ygf.yj202588.top

JS:   get name() { return this._name; }
来源：http://iaa.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://khq.aibaodan.cn

Java: public String getName() { return name; }
来源：http://itd.gotoacloud.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ult.0kj1m.cn

Ruby: attr_accessor :name
来源：http://owx.mhx1999.top

C#:   public string Name { get; set; }
来源：http://esf.havefunace.top

[G12] 对象转字符串
来源：http://urz.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://yfb.shuidangran.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://bau.52xcode.cn

JS:   toString() { return this.name; }
来源：http://ftz.jianghu66.top

TS:   toString(): string { return this.name; }
来源：http://tmx.havefunace.top

Java: @Override public String toString() { return name; }
来源：http://hws.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://mrf.cdnleiting.top

Ruby: def to_s; @name; end
来源：http://nhk.shanyushiyangtech.top

C#:   public override string ToString() => Name;
来源：http://jsz.haohaochexian.top

[G13] 判断对象类型
来源：http://bhe.chenzaomai.com

Py:   isinstance(u, User)
来源：http://ckr.tanke756.top

PHP:  $u instanceof User
来源：http://doh.yangfankeji.com

JS:   u instanceof User
来源：http://rsp.gogol.net.cn

TS:   u instanceof User
来源：http://cbi.fanxiaobao.xyz

Java: u instanceof User
来源：http://dcn.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xjp.jqgfzy.top

Ruby: u.is_a?(User)
来源：http://iuq.chenlongwang.top

C#:   u is User
来源：http://erf.havefunace.top

[G14] 数据类 / record
来源：http://zir.hesvh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qrg.hcnkem.com

PHP:  // 用 readonly 属性模拟
来源：http://max.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ubu.shanyushiyangtech.top

TS:   type User = { name: string; age: number };
来源：http://ugk.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://ycz.dashuyun.cn

Go:   type User struct { Name string; Age int }
来源：http://tmv.zhoulong.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cfw.hnqzz.top

C#:   record User(string Name, int Age);
来源：http://eua.ppjwa.cn

[G15] 枚举
来源：http://dnd.epnwcf.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://skf.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://uvq.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://umy.yonumen.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jgb.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://far.shangyingyoupin.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lew.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://vfr.jinqigfzy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fch.ivvv.top

[G16] 对象转数组 / 字典
来源：http://oze.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uhx.sysykeji.top

PHP:  get_object_vars($obj);
来源：http://zef.ywan-chungtsiang.top

JS:   Object.entries(obj)
来源：http://xpp.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://yag.cdnleiting.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wae.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://meg.wangdashe.top

Ruby: obj.instance_variables
来源：http://mrv.shanyushiyangtech.top

C#:   // 用反射或 System.Text.Json
来源：http://pwj.pycfn.com

================================================================================
来源：http://vbp.cashguo.top

H. 异常与错误处理
来源：http://ocv.hesvh.cn

================================================================================
来源：http://daq.guannengcc.top

[H01] try / catch 基础
来源：http://gjx.shanyushiyangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cux.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aqm.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uvo.zhixingplan.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kxr.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwx.gogol.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://otn.jlsjyb.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jem.chenjidiqi.icu

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xlf.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://vea.9152youxi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dme.nanxinkj.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://vaq.xziqi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yly.shzxlz.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pzi.aibaodan.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dsf.sufxvd.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nos.shanyushiyangtech.top

Ruby: begin; f; ensure; cleanup; end
来源：http://znb.gotoacloud.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bkr.jinqigfzy.top

[H03] 主动抛出异常
来源：http://vqj.hnxiangtu.top

Py:   raise ValueError("错误信息")
来源：http://zwu.andypj.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://seb.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://qkl.hesvh.cn

TS:   throw new Error("错误信息");
来源：http://icu.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://vec.jqgfzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wyc.iojbl.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oce.yj202588.top

C#:   throw new ArgumentException("错误信息");
来源：http://prm.cucudq.cn

[H04] 自定义异常类型
来源：http://ywn.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://xvt.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oux.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://wyb.nanxinkj.top

TS:   class MyError extends Error {}
来源：http://stj.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://yxu.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://she.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://sex.aizwys.cn

C#:   class MyException : Exception {}
来源：http://hho.bbcook.cn

[H05] 捕获特定类型
来源：http://egr.ehwqpu.com

Py:   except ValueError as e:
来源：http://kpw.shanyushiyangkeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tim.yj202588.top

JS:   if (e instanceof TypeError) {}
来源：http://pvx.zhiwuduotai.top

TS:   if (e instanceof TypeError) {}
来源：http://wtx.xylfe.cn

Java: catch (IOException | SQLException e) {}
来源：http://zmq.zhongyouzk.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zqv.zhongyouzk.top

Ruby: rescue ArgumentError => e
来源：http://lov.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mph.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://hic.aibaodan.cn

Py:   value = d.get("k") or default
来源：http://zud.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gxe.mhx1999.top

JS:   obj?.a?.b;  d ?? default
来源：http://vlm.yfazqb.com

TS:   obj?.a?.b;  d ?? default
来源：http://pbu.fanxiaobao.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eji.sxryk.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nfy.yfazqb.com

Ruby: d&.dig(:a, :b)
来源：http://irz.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://kzf.bbcook.cn

[H07] 断言
来源：http://kbo.zhoulong.xyz

Py:   assert x > 0, "必须为正"
来源：http://sub.vehdjk.com

PHP:  assert($x > 0);
来源：http://wrd.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://ykx.ehwqpu.com

TS:   console.assert(x > 0);
来源：http://xlm.yj20258888.top

Java: assert x > 0 : "必须为正";
来源：http://czc.fanxiaobao.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pgm.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vmu.uphjek.com

C#:   Debug.Assert(x > 0);
来源：http://tcd.yj20258888.top

[H08] 获取错误信息与堆栈
来源：http://fys.yj202588.top

Py:   str(e);  traceback.format_exc()
来源：http://kbe.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gro.xinyue.icu

JS:   e.message;  e.stack
来源：http://vfq.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bcs.jinqigfzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wkp.zhaomingkeji.xyz

Go:   err.Error()
来源：http://noj.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://bwt.cdnleiting.top

C#:   e.Message;  e.StackTrace
来源：http://gwr.pycfn.com

[H09] 带错误码的异常
来源：http://yby.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eya.ybcxt.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wla.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zmb.mhx1999.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kox.shuidangran.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lvr.tian-w.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bam.c1oappe.top

Ruby: raise MyError.new("fail", 500)
来源：http://gsx.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iir.sufxvd.cn

[H10] 资源自动释放
来源：http://oit.9152youxi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wmv.9152youxi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wqu.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ymi.xinyue.icu

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wme.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://riq.9152youxi.cn

Go:   defer f.Close()
来源：http://xcg.hfpthk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rnq.tanke756.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zcb.yueranfly.top

================================================================================
来源：http://uvz.hammf.cn

I. 正则表达式
来源：http://nwj.ppjwa.cn

================================================================================
来源：http://iof.tarul.cn

[I01] 判断是否匹配
来源：http://njp.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tjk.c1oappe.top

PHP:  preg_match('/\d+/', $s);
来源：http://ugz.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://wpn.cucudq.cn

TS:   /\d+/.test(s)
来源：http://jsf.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yns.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://noc.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://cvz.sweek.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://omj.jinqigufen.top

[I02] 提取所有匹配
来源：http://xur.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://uzb.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xqp.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uka.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://byr.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hbg.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yts.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://vgg.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vre.havefunace.top

[I03] 提取捕获分组
来源：http://xrg.jinqigufen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nqx.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mbi.mhx1999.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kxv.birdmap.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wwe.ctjpmb.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uoi.andypj.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://chc.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cwk.vehdjk.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lic.316326.xyz

[I04] 正则替换
来源：http://aok.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rlk.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://taf.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://emn.iojbl.cn

TS:   s.replace(/\d+/g, "#")
来源：http://phy.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://gur.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://orb.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cym.c1oappe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pzr.jyoumei.cn

[I05] 按正则拆分
来源：http://ntd.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://muq.tanke756.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wio.xinyue.icu

JS:   s.split(/\s*,\s*/)
来源：http://ipv.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://poq.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://oph.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nzf.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kty.52xcode.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nmn.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fcu.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nhl.yueranfly.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mmo.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rpn.vqdsnc.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fvc.havefunace.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fhk.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://emr.xuetiantiany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lbh.shanyushiyangtech.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://twe.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://rqo.nwbrower.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zvg.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://obb.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://anj.jqgufenzy.top

TS:   /error/gim
来源：http://vgq.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jje.aibaodan.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sov.fanxiaobao.xyz

Ruby: s.scan(/error/i)
来源：http://fna.fengsongda.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cwd.xuetiantiany.cn

[I08] 贪婪与非贪婪匹配
来源：http://hcj.jqgufenzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://czp.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://neq.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nwz.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jvy.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ihx.zdbjq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://khx.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://opk.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yjz.ppjwa.cn

================================================================================
来源：http://fnn.9152youxi.cn

J. 日期与时间
来源：http://uyv.aibaodan.cn

================================================================================
来源：http://bqk.pycfn.com

[J01] 获取当前时间
来源：http://fus.ybcxt.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dnr.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://our.yfazqb.com

JS:   new Date();  Date.now()
来源：http://boy.aibaodan.cn

TS:   new Date();  Date.now()
来源：http://qyj.cheryme.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ssh.chenlongwang.top

Go:   time.Now()
来源：http://vkc.cucudq.cn

Ruby: Time.now
来源：http://sti.sweek.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pge.zhoulong.xyz

[J02] 格式化输出
来源：http://kbp.zhixingplan.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wve.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hzk.tian-w.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lvi.cashguo.top

TS:   d.toISOString()
来源：http://zfe.jinghuilouyu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fbx.yonumen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kca.ivvv.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://djr.chenlongwang.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ima.nanxinkj.top

[J03] 字符串解析为日期
来源：http://qba.birdmap.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sbo.smart0.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tzg.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://wai.zhiwuduotai.top

TS:   new Date("2024-01-02")
来源：http://ffq.zhoulong.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://ils.ydjk.org.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ezg.mhx1999.top

Ruby: Date.parse("2024-01-02")
来源：http://fnn.gzhubu.top


<!-- 参考信息 -->