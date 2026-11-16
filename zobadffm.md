代发 wailian999

Ruby: @name = "x"
来源：http://ngg.chenjidiqi.icu

C#:   public string Name { get; set; } = "x";
来源：http://mos.zdbjq.cn

[G04] 定义方法
来源：http://eox.pengpengdd.cyou

Py:   def greet(self): return self.name
来源：http://pov.shuidangran.top

PHP:  public function greet(): string { return $this->name; }
来源：http://zrf.316326.xyz

JS:   greet() { return this.name; }
来源：http://wnu.hnqzz.top

TS:   greet(): string { return this.name; }
来源：http://ret.yj202588.top

Java: String greet() { return name; }
来源：http://kzs.hongshengwenyu.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://mnu.cqqwz.cn

Ruby: def greet; @name; end
来源：http://axx.zhixingplan.top

C#:   public string Greet() => Name;
来源：http://fkz.fanxiaobao.xyz

[G05] 继承
来源：http://nrh.zdqjudy.top

Py:   class Admin(User): pass
来源：http://fne.ywan-chungtsiang.top

PHP:  class Admin extends User {}
来源：http://zuz.mhx1999.top

JS:   class Admin extends User {}
来源：http://juj.ctjpmb.com

TS:   class Admin extends User {}
来源：http://tas.nanxuanxn.top

Java: class Admin extends User {}
来源：http://fxt.havefunace.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tzc.nwbrower.top

Ruby: class Admin < User; end
来源：http://fhy.tanke756.top

C#:   class Admin : User {}
来源：http://sva.hnqzz.top

[G06] 重写方法
来源：http://saz.jinghuilouyu.cn

Py:   def greet(self): return "admin"
来源：http://dkp.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://thg.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://ban.yfazqb.com

TS:   greet(): string { return "admin"; }
来源：http://ctc.dashuyun.cn

Java: @Override String greet() { return "admin"; }
来源：http://rll.cucudq.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qqf.yonumen.top

Ruby: def greet; "admin"; end
来源：http://pzk.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://rmd.chenjidiqi.icu

[G07] 调用父类方法
来源：http://yhd.mhx1999.top

Py:   super().greet()
来源：http://akn.yj202588.top

PHP:  parent::greet();
来源：http://ofk.ppjwa.cn

JS:   super.greet();
来源：http://xst.ybcxt.top

TS:   super.greet();
来源：http://kwy.xuanzx.com

Java: super.greet();
来源：http://aep.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jzc.xuetiantiany.cn

Ruby: super
来源：http://btn.hfpthk.cn

C#:   base.Greet();
来源：http://byk.hongshengwenyu.top

[G08] 静态方法与属性
来源：http://ajj.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dbb.gaohongyu789.top

PHP:  public static function f() {}
来源：http://xim.aibaodan.cn

JS:   static f() {}
来源：http://iyh.cucudq.cn

TS:   static f(): void {}
来源：http://aqr.pycfn.com

Java: static void f() {}
来源：http://zcl.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://eek.zhaomingkeji.xyz

Ruby: def self.f; end
来源：http://dcr.havefunace.top

C#:   public static void F() {}
来源：http://vce.c1oappe.top

[G09] 接口 / 抽象类
来源：http://ebl.tanke756.top

Py:   from abc import ABC, abstractmethod
来源：http://lwo.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iei.hysaishi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vui.jinyuanbaomall.cn

TS:   interface Shape { area(): number; }
来源：http://zwy.52xcode.cn

Java: interface Shape { double area(); }
来源：http://neo.yuanzhike.top

Go:   type Shape interface { Area() float64 }
来源：http://rlf.smart0.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hfz.fengsongda.top

C#:   interface IShape { double Area(); }
来源：http://hge.sxryk.cn

[G10] 访问控制
来源：http://xdl.zdqjudy.top

Py:   约定 _protected / __private（不强制）
来源：http://nfo.fehbvm.com

PHP:  public / protected / private
来源：http://ilg.cucudq.cn

JS:   #private 字段；其余公开
来源：http://xmf.jyoumei.cn

TS:   public / protected / private
来源：http://uca.andypj.xyz

Java: public / protected / private / 默认包级
来源：http://wmr.wangshuangyany.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rbx.meibo888.top

Ruby: public / protected / private
来源：http://mdw.iojbl.cn

C#:   public / protected / private / internal
来源：http://azq.sweek.top

[G11] getter / setter
来源：http://ttx.yj20258888.top

Py:   @property 与 @x.setter
来源：http://zbt.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://oyo.jyoumei.cn

JS:   get name() { return this._name; }
来源：http://vfn.yj20258888.top

TS:   get name(): string { return this._name; }
来源：http://bei.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://eav.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://amf.cdnleiting.top

Ruby: attr_accessor :name
来源：http://mjk.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://fvz.birdmap.top

[G12] 对象转字符串
来源：http://wbo.ivvv.top

Py:   def __str__(self): return self.name
来源：http://ljt.52xcode.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://whd.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://vbm.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://vbv.zhoulong.xyz

Java: @Override public String toString() { return name; }
来源：http://ktw.zycfv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mlk.cheryme.top

Ruby: def to_s; @name; end
来源：http://udj.yanxiufei.cn

C#:   public override string ToString() => Name;
来源：http://loh.aibaodan.cn

[G13] 判断对象类型
来源：http://fkx.yuxming.cn

Py:   isinstance(u, User)
来源：http://ece.ivvv.top

PHP:  $u instanceof User
来源：http://adq.zhengqikj.top

JS:   u instanceof User
来源：http://sod.zhengqikj.top

TS:   u instanceof User
来源：http://nwb.9152youxi.cn

Java: u instanceof User
来源：http://cna.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jrl.xziqi.cn

Ruby: u.is_a?(User)
来源：http://yvf.xinyue.icu

C#:   u is User
来源：http://jxg.jianghu66.top

[G14] 数据类 / record
来源：http://ohn.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pdk.sxryk.cn

PHP:  // 用 readonly 属性模拟
来源：http://yui.hfpthk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uci.tarul.cn

TS:   type User = { name: string; age: number };
来源：http://mpf.zdbjq.cn

Java: record User(String name, int age) {}
来源：http://ihd.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://wze.316326.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sdc.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://bmj.hongshengwenyu.top

[G15] 枚举
来源：http://zyh.smart0.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://acu.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bvs.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vdv.yj20258888.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dms.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://biz.haohaochexian.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vri.xuetiantiany.cn

Ruby: Color = %i[red green].freeze
来源：http://emu.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pow.hongshengwenyu.top

[G16] 对象转数组 / 字典
来源：http://eex.sysykeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rhp.redwolf501.top

PHP:  get_object_vars($obj);
来源：http://jfg.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://eax.tian-w.cn

TS:   Object.entries(obj)
来源：http://oor.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mnj.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://yqy.yueranfly.top

Ruby: obj.instance_variables
来源：http://hif.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://wfd.nanxinkj.top

================================================================================
来源：http://naq.jinqigufen.top

H. 异常与错误处理
来源：http://unq.jinqigfzy.top

================================================================================
来源：http://vkm.ivvv.top

[H01] try / catch 基础
来源：http://zuy.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fvf.jqgufenzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bqd.daxiang520.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lch.ybcxt.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cay.fengsongda.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://awm.tian-w.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sfp.hnqzz.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jxv.birdmap.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://glb.ehwqpu.com

[H02] finally / ensure 收尾
来源：http://jyy.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://kdz.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hxk.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ddm.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gmd.jqgfzy.top

Java: try { f(); } finally { cleanup(); }
来源：http://gfb.jinqigfzy.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://eec.shangyingyoupin.top

Ruby: begin; f; ensure; cleanup; end
来源：http://pno.yonumen.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://aeg.guowangkeji.top

[H03] 主动抛出异常
来源：http://erf.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://zez.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fib.tanke756.top

JS:   throw new Error("错误信息");
来源：http://tnr.zhijiandao.cn

TS:   throw new Error("错误信息");
来源：http://wtn.snrcjt.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lfh.jianghu66.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bsw.yueranfly.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sjq.smart0.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://uep.jiagoushi.top

[H04] 自定义异常类型
来源：http://uas.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://hsz.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rzj.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://ikm.pycfn.com

TS:   class MyError extends Error {}
来源：http://fgy.cheryme.top

Java: class MyException extends RuntimeException {}
来源：http://ahy.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tmd.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://dpj.bjfxy.top

C#:   class MyException : Exception {}
来源：http://ern.gogol.net.cn

[H05] 捕获特定类型
来源：http://ybj.hnqzz.top

Py:   except ValueError as e:
来源：http://fnf.yonumen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zxh.guannengcc.top

JS:   if (e instanceof TypeError) {}
来源：http://xwz.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://foe.wangshuangyany.cn

Java: catch (IOException | SQLException e) {}
来源：http://exx.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://olu.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://rsy.meibo888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iwm.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://hhk.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://jxt.vqdsnc.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vdd.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://nzj.smart0.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://fzy.gaohongyu789.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eow.xingfuxueyuan.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://wze.shuidangran.top

Ruby: d&.dig(:a, :b)
来源：http://jdm.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://efk.fzhhl.top

[H07] 断言
来源：http://jle.fanxiaobao.xyz

Py:   assert x > 0, "必须为正"
来源：http://uzh.cashguo.top

PHP:  assert($x > 0);
来源：http://sld.cheryme.top

JS:   console.assert(x > 0);
来源：http://bas.316326.xyz

TS:   console.assert(x > 0);
来源：http://ymu.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://xcm.yonumen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mik.fanxiaobao.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://vty.0kj1m.cn

C#:   Debug.Assert(x > 0);
来源：http://fxo.tian-w.cn

[H08] 获取错误信息与堆栈
来源：http://eta.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://xfv.xylfe.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pmv.vqdsnc.cn

JS:   e.message;  e.stack
来源：http://tgb.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mhb.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cxe.pengpengdd.cyou

Go:   err.Error()
来源：http://hvp.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://tgk.jinqigufen.top

C#:   e.Message;  e.StackTrace
来源：http://qyp.gogol.net.cn

[H09] 带错误码的异常
来源：http://wtn.andypj.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xzh.quarkkingdee.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://jly.xuanzx.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cli.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pwz.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zhf.shuidangran.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://goz.dashuyun.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hhd.jinqigufen.top

C#:   // 自定义异常类中加 Code 属性
来源：http://mte.fktsv.cn

[H10] 资源自动释放
来源：http://ktw.zdqjudy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://nek.yuxming.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ddx.yongpay.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nfu.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uzh.uphjek.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://toq.zhoulong.xyz

Go:   defer f.Close()
来源：http://gnn.ppjwa.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://etw.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bar.yueranfly.top

================================================================================
来源：http://yck.ydjk.org.cn

I. 正则表达式
来源：http://qrv.aizwys.cn

================================================================================
来源：http://idm.snrcjt.cn

[I01] 判断是否匹配
来源：http://agw.yonumen.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xfl.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://cuw.cashguo.top

JS:   /\d+/.test(s)
来源：http://ozm.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://iph.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iiv.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://and.mhx1999.top

Ruby: s.match?(/\d+/)
来源：http://cki.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ohj.ehwqpu.com

[I02] 提取所有匹配
来源：http://psf.yonumen.top

Py:   re.findall(r"\d+", s)
来源：http://orz.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nqi.tanke756.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zbi.hammf.cn

TS:   s.match(/\d+/g)
来源：http://arp.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://skx.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zlo.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://nla.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://imj.dianchejie.cn

[I03] 提取捕获分组
来源：http://ntl.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aqg.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kep.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dyb.andypj.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pfn.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tpr.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yiu.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yff.havefunace.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wbj.hnxiangtu.top

[I04] 正则替换
来源：http://wxg.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qgb.fzhhl.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cbn.zhixingplan.top

JS:   s.replace(/\d+/g, "#")
来源：http://wil.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://hub.yj20258.top

Java: s.replaceAll("\\d+", "#")
来源：http://cjv.ivvv.top

Go:   re.ReplaceAllString(s, "#")
来源：http://yjc.jinqigufen.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nwu.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://htc.hfpthk.cn

[I05] 按正则拆分
来源：http://bfr.ivvv.top

Py:   re.split(r"\s*,\s*", s)
来源：http://uvd.jlsjyb.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wdt.sjlbkw.cn

JS:   s.split(/\s*,\s*/)
来源：http://ziq.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://vuy.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://pny.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ygi.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vbd.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hwn.tanke756.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://chx.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kue.zhengqikj.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zlw.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jhr.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fgc.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hdv.yj20258.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rdo.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ern.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://epw.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://yqt.aibaodan.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yah.yonumen.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bxh.yuanzhike.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tnq.havefunace.top

TS:   /error/gim
来源：http://jec.andypj.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zde.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wqs.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://yyk.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zen.ydzc1.top

[I08] 贪婪与非贪婪匹配
来源：http://bxx.fktsv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdt.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ydx.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ahe.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zas.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tku.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://coy.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://asm.0kj1m.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tlb.shuidangran.top

================================================================================
来源：http://zaa.xuanzx.com

J. 日期与时间
来源：http://ogb.yj20258888.top

================================================================================
来源：http://hvm.wangdashe.top

[J01] 获取当前时间
来源：http://dus.daria6918.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hqv.yj20258.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dnr.316326.xyz

JS:   new Date();  Date.now()
来源：http://nvi.hfpthk.cn

TS:   new Date();  Date.now()
来源：http://urc.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://akx.ctjpmb.com

Go:   time.Now()
来源：http://sli.yj20258888.top

Ruby: Time.now
来源：http://num.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yty.shzxlz.cn

[J02] 格式化输出
来源：http://por.yueranfly.top


<!-- 参考信息 -->