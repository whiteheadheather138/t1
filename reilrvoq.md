代发 wailian999

Py:   class Admin(User): pass
来源：http://ect.xuanzx.com

PHP:  class Admin extends User {}
来源：http://xmi.jiagoushi.top

JS:   class Admin extends User {}
来源：http://ypd.mhx1999.top

TS:   class Admin extends User {}
来源：http://aib.shangyingyoupin.top

Java: class Admin extends User {}
来源：http://rvz.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vfx.yonumen.top

Ruby: class Admin < User; end
来源：http://coo.ehwqpu.com

C#:   class Admin : User {}
来源：http://gkr.guowangkeji.top

[G06] 重写方法
来源：http://xft.cqqwz.cn

Py:   def greet(self): return "admin"
来源：http://iyo.cdnleiting.top

PHP:  public function greet(): string { return "admin"; }
来源：http://rpm.xingfuxueyuan.xyz

JS:   greet() { return "admin"; }
来源：http://vch.shuidangran.top

TS:   greet(): string { return "admin"; }
来源：http://eyj.zdqjudy.top

Java: @Override String greet() { return "admin"; }
来源：http://mlw.ydzc1.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ikb.zhaomingkeji.xyz

Ruby: def greet; "admin"; end
来源：http://cgt.sxryk.cn

C#:   public override string Greet() => "admin";
来源：http://vej.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://bod.daxiang520.top

Py:   super().greet()
来源：http://nqp.yj20258888.top

PHP:  parent::greet();
来源：http://ova.jyoumei.cn

JS:   super.greet();
来源：http://iwc.cdnleiting.top

TS:   super.greet();
来源：http://ynk.xylfe.cn

Java: super.greet();
来源：http://nqk.shanyushiyangtech.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vdj.fzhhl.top

Ruby: super
来源：http://dbp.cucudq.cn

C#:   base.Greet();
来源：http://yie.hnqzz.top

[G08] 静态方法与属性
来源：http://bdy.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ybj.zdbjq.cn

PHP:  public static function f() {}
来源：http://zfv.sjlbkw.cn

JS:   static f() {}
来源：http://bos.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://lgz.zdbjq.cn

Java: static void f() {}
来源：http://yzy.cucudq.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cuy.vehdjk.com

Ruby: def self.f; end
来源：http://ulx.chenzaomai.com

C#:   public static void F() {}
来源：http://ofu.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://qzf.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://xwb.gzhubu.top

PHP:  interface Shape { public function area(): float; }
来源：http://oqv.fengsongda.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://mue.aizwys.cn

TS:   interface Shape { area(): number; }
来源：http://ozf.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://nki.zhoulong.xyz

Go:   type Shape interface { Area() float64 }
来源：http://qog.andypj.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://flm.daria6918.cn

C#:   interface IShape { double Area(); }
来源：http://chc.yj20258888.top

[G10] 访问控制
来源：http://lec.jianghu66.top

Py:   约定 _protected / __private（不强制）
来源：http://rvv.dashuyun.cn

PHP:  public / protected / private
来源：http://jco.aizwys.cn

JS:   #private 字段；其余公开
来源：http://vap.kuanghao11.cn

TS:   public / protected / private
来源：http://zlp.yuanzhike.top

Java: public / protected / private / 默认包级
来源：http://dat.cucudq.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://clx.aibaodan.cn

Ruby: public / protected / private
来源：http://irc.fengsongda.top

C#:   public / protected / private / internal
来源：http://psk.shangyingyoupin.top

[G11] getter / setter
来源：http://lxg.hcnkem.com

Py:   @property 与 @x.setter
来源：http://cmm.hammf.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ald.yonumen.top

JS:   get name() { return this._name; }
来源：http://gmh.pycfn.com

TS:   get name(): string { return this._name; }
来源：http://psh.316326.xyz

Java: public String getName() { return name; }
来源：http://lrv.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://etj.zdbjq.cn

Ruby: attr_accessor :name
来源：http://agp.sweek.top

C#:   public string Name { get; set; }
来源：http://uay.9152youxi.cn

[G12] 对象转字符串
来源：http://ros.316326.xyz

Py:   def __str__(self): return self.name
来源：http://nlp.fktsv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zat.sxryk.cn

JS:   toString() { return this.name; }
来源：http://tgg.yongpay.top

TS:   toString(): string { return this.name; }
来源：http://xdc.epnwcf.com

Java: @Override public String toString() { return name; }
来源：http://fck.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://zix.zhoulong.xyz

Ruby: def to_s; @name; end
来源：http://eoe.jiagoushi.top

C#:   public override string ToString() => Name;
来源：http://sxq.mhx1999.top

[G13] 判断对象类型
来源：http://mex.jlsjyb.cn

Py:   isinstance(u, User)
来源：http://fwv.chenzaomai.com

PHP:  $u instanceof User
来源：http://oyr.sjlbkw.cn

JS:   u instanceof User
来源：http://kym.redwolf501.top

TS:   u instanceof User
来源：http://dvi.birdmap.top

Java: u instanceof User
来源：http://nne.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dsg.gzhubu.top

Ruby: u.is_a?(User)
来源：http://kft.sysykeji.top

C#:   u is User
来源：http://pyd.fzhhl.top

[G14] 数据类 / record
来源：http://jhb.zycfv.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vsx.meibo888.top

PHP:  // 用 readonly 属性模拟
来源：http://qkr.jqgufenzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://kmx.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://qcu.xuanzx.com

Java: record User(String name, int age) {}
来源：http://raa.shanyushiyangtech.top

Go:   type User struct { Name string; Age int }
来源：http://cup.meibo888.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://izf.cucudq.cn

C#:   record User(string Name, int Age);
来源：http://xtf.yvedp.cn

[G15] 枚举
来源：http://qob.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://irl.andypj.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://wdh.shuidangran.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ymk.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sti.ehwqpu.com

Java: enum Color { RED, GREEN }
来源：http://kmk.chenlongwang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://afp.havefunace.top

Ruby: Color = %i[red green].freeze
来源：http://foc.zycfv.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bfk.ehwqpu.com

[G16] 对象转数组 / 字典
来源：http://tsb.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://efu.zdqjudy.top

PHP:  get_object_vars($obj);
来源：http://kzu.cqqwz.cn

JS:   Object.entries(obj)
来源：http://bid.vqdsnc.cn

TS:   Object.entries(obj)
来源：http://aqv.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pvs.shuidangran.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://xrb.shzxlz.cn

Ruby: obj.instance_variables
来源：http://pro.vqdsnc.cn

C#:   // 用反射或 System.Text.Json
来源：http://pqq.vqdsnc.cn

================================================================================
来源：http://axm.xziqi.cn

H. 异常与错误处理
来源：http://yqi.quarkkingdee.top

================================================================================
来源：http://hkg.zhoulong.xyz

[H01] try / catch 基础
来源：http://rsl.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jph.mhx1999.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lbu.dashuyun.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mzu.andypj.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ppg.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hjf.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pav.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hbz.yueranfly.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ytj.svipenyu.cn

[H02] finally / ensure 收尾
来源：http://aof.nanxuanxn.top

Py:   try: f()⏎finally: cleanup()
来源：http://xbo.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wgg.zhiwuduotai.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lct.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nhz.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nsv.c1oappe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://qev.9152youxi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iir.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://qes.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://dmm.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://vrx.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pad.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://atv.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://liv.zhengqikj.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://hsy.xuetiantiany.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://egt.fengsongda.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cpr.kuanghao11.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vcz.zdqjudy.top

[H04] 自定义异常类型
来源：http://ypv.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://adw.shanyushiyangtech.top

PHP:  class MyError extends RuntimeException {}
来源：http://bsx.cqqwz.cn

JS:   class MyError extends Error {}
来源：http://joi.yuxming.cn

TS:   class MyError extends Error {}
来源：http://ank.gzhubu.top

Java: class MyException extends RuntimeException {}
来源：http://vix.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jrp.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://xiz.guannengcc.top

C#:   class MyException : Exception {}
来源：http://fvi.hfpthk.cn

[H05] 捕获特定类型
来源：http://uxh.vqdsnc.cn

Py:   except ValueError as e:
来源：http://krs.316326.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gdo.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://kup.sxryk.cn

TS:   if (e instanceof TypeError) {}
来源：http://tib.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://rsk.ydjk.org.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jui.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://jnc.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zds.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://ulh.daria6918.cn

Py:   value = d.get("k") or default
来源：http://rgw.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uhi.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://stt.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://iyw.yongpay.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ptc.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://egp.tanke756.top

Ruby: d&.dig(:a, :b)
来源：http://phq.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://edr.fehbvm.com

[H07] 断言
来源：http://isk.cashguo.top

Py:   assert x > 0, "必须为正"
来源：http://jqw.epnwcf.com

PHP:  assert($x > 0);
来源：http://jft.aibaodan.cn

JS:   console.assert(x > 0);
来源：http://nyi.vqdsnc.cn

TS:   console.assert(x > 0);
来源：http://fyj.jianghu66.top

Java: assert x > 0 : "必须为正";
来源：http://idc.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zsi.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://bwx.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://aqr.cucudq.cn

[H08] 获取错误信息与堆栈
来源：http://dyd.jinqigufen.top

Py:   str(e);  traceback.format_exc()
来源：http://glk.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mfe.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://myg.shanyushiyangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ihn.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ykj.fktsv.cn

Go:   err.Error()
来源：http://whh.nwbrower.top

Ruby: e.message;  e.backtrace
来源：http://fru.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://tol.sufxvd.cn

[H09] 带错误码的异常
来源：http://mas.chenlongwang.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://avr.mhx1999.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://frx.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hnc.meibo888.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wid.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ubj.bjfxy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jwu.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://rty.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://irg.guowangkeji.top

[H10] 资源自动释放
来源：http://jvw.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://jpx.zhaomingkeji.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ssg.xingfuxueyuan.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ibw.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zzz.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ueq.shzxlz.cn

Go:   defer f.Close()
来源：http://wls.jlsjyb.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uet.guannengcc.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gqv.yuxming.cn

================================================================================
来源：http://jox.redwolf501.top

I. 正则表达式
来源：http://fbs.dashuyun.cn

================================================================================
来源：http://hxq.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://gzz.fktsv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bib.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jyy.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://gqg.hnxiangtu.top

TS:   /\d+/.test(s)
来源：http://igq.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hyn.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wgg.dianchejie.cn

Ruby: s.match?(/\d+/)
来源：http://idw.jqgfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mdy.jinqigfzy.top

[I02] 提取所有匹配
来源：http://wom.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://dwu.gaohongyu789.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sgl.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://piz.yueranfly.top

TS:   s.match(/\d+/g)
来源：http://ocq.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xuu.yuxming.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tqu.fengsongda.top

Ruby: s.scan(/\d+/)
来源：http://opw.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ewd.316326.xyz

[I03] 提取捕获分组
来源：http://qev.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qbc.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dbp.xylfe.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fkq.cqqwz.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sja.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bll.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://acc.jinyuanbaomall.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dgz.guannengcc.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nno.nwbrower.top

[I04] 正则替换
来源：http://svr.fehbvm.com

Py:   re.sub(r"\d+", "#", s)
来源：http://yqg.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vwz.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eji.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://ryi.yfazqb.com

Java: s.replaceAll("\\d+", "#")
来源：http://qxx.wangdashe.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uvt.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://etb.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ivg.zdqjudy.top

[I05] 按正则拆分
来源：http://yjz.sweek.top

Py:   re.split(r"\s*,\s*", s)
来源：http://gvi.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pqs.cheryme.top

JS:   s.split(/\s*,\s*/)
来源：http://stk.jinqigufen.top

TS:   s.split(/\s*,\s*/)
来源：http://mjb.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://zha.quarkkingdee.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://upe.pycfn.com

Ruby: s.split(/\s*,\s*/)
来源：http://vdh.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://clx.jinqigfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tbm.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dco.iojbl.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://trr.ctjpmb.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ndb.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kir.jqgfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oak.gzhubu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oaj.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jps.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xqi.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://ezn.vehdjk.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xhw.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://soe.chenlongwang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aov.uphjek.com

TS:   /error/gim
来源：http://bcg.yueranfly.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rzx.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mas.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://yza.jinyuanbaomall.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rmk.gzhubu.top

[I08] 贪婪与非贪婪匹配
来源：http://fel.hcnkem.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hmn.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cwx.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mpi.hammf.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nhd.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vwl.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tra.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hlq.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mqj.jinyuanbaomall.cn

================================================================================
来源：http://fqk.birdmap.top

J. 日期与时间
来源：http://fxd.aibaodan.cn

================================================================================
来源：http://wct.ydjk.org.cn

[J01] 获取当前时间
来源：http://urr.jqgfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://cho.zhongyouzk.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zhy.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://tta.zhiwuduotai.top

TS:   new Date();  Date.now()
来源：http://bcx.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dwj.fzhhl.top

Go:   time.Now()
来源：http://wyo.yj20258.top

Ruby: Time.now
来源：http://ekg.tarul.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uix.yj202588.top

[J02] 格式化输出
来源：http://zaj.meibo888.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yoy.hfpthk.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://boy.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ywo.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://zqj.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hgr.dianchejie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://okr.gotoacloud.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nou.sjlbkw.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ccc.tanke756.top

[J03] 字符串解析为日期
来源：http://ljs.wangshuangyany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rvq.nanxuanxn.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://usj.cqqwz.cn

JS:   new Date("2024-01-02")
来源：http://jxc.mhx1999.top


<!-- 参考信息 -->