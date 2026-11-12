代发 wailian999

Ruby: @name = "x"
来源：http://xlj.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://psb.jiagoushi.top

[G04] 定义方法
来源：http://xsk.yj20258.top

Py:   def greet(self): return self.name
来源：http://pux.jianghu66.top

PHP:  public function greet(): string { return $this->name; }
来源：http://brn.cheryme.top

JS:   greet() { return this.name; }
来源：http://mrh.xylfe.cn

TS:   greet(): string { return this.name; }
来源：http://tkp.iojbl.cn

Java: String greet() { return name; }
来源：http://ogj.tian-w.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mot.havefunace.top

Ruby: def greet; @name; end
来源：http://lgy.hfpthk.cn

C#:   public string Greet() => Name;
来源：http://wck.bbcook.cn

[G05] 继承
来源：http://tox.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://tdi.yj20258888.top

PHP:  class Admin extends User {}
来源：http://bvl.cucudq.cn

JS:   class Admin extends User {}
来源：http://kjn.sjlbkw.cn

TS:   class Admin extends User {}
来源：http://tkl.yueranfly.top

Java: class Admin extends User {}
来源：http://hgg.c1oappe.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vve.guowangkeji.top

Ruby: class Admin < User; end
来源：http://tlb.jianghu66.top

C#:   class Admin : User {}
来源：http://ebr.shanyushiyangkeji.top

[G06] 重写方法
来源：http://dyz.aibaodan.cn

Py:   def greet(self): return "admin"
来源：http://dio.haohaochexian.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zzc.yonumen.top

JS:   greet() { return "admin"; }
来源：http://uzs.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://ewc.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://vxi.hesvh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dyo.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://ldv.shanyushiyangkeji.top

C#:   public override string Greet() => "admin";
来源：http://koe.chenlongwang.top

[G07] 调用父类方法
来源：http://vbw.xylfe.cn

Py:   super().greet()
来源：http://zzl.wangdashe.top

PHP:  parent::greet();
来源：http://hoa.jinghuilouyu.cn

JS:   super.greet();
来源：http://xpt.fanxiaobao.xyz

TS:   super.greet();
来源：http://zfk.ehwqpu.com

Java: super.greet();
来源：http://ilj.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ygg.guannengcc.top

Ruby: super
来源：http://kod.smart0.xyz

C#:   base.Greet();
来源：http://qtv.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://cds.guowangkeji.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zbu.xziqi.cn

PHP:  public static function f() {}
来源：http://bdj.vqdsnc.cn

JS:   static f() {}
来源：http://xpe.ivvv.top

TS:   static f(): void {}
来源：http://mcf.ctjpmb.com

Java: static void f() {}
来源：http://znq.0kj1m.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://khy.tanke756.top

Ruby: def self.f; end
来源：http://jea.yuanzhike.top

C#:   public static void F() {}
来源：http://egc.daria6918.cn

[G09] 接口 / 抽象类
来源：http://lqe.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://xco.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://baq.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://djm.ydzc1.top

TS:   interface Shape { area(): number; }
来源：http://tsl.sxryk.cn

Java: interface Shape { double area(); }
来源：http://rqe.xuanzx.com

Go:   type Shape interface { Area() float64 }
来源：http://cgy.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xtg.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://knx.ctjpmb.com

[G10] 访问控制
来源：http://xzp.ydzc1.top

Py:   约定 _protected / __private（不强制）
来源：http://hiy.nanxinkj.top

PHP:  public / protected / private
来源：http://dbg.yj20258.top

JS:   #private 字段；其余公开
来源：http://pqw.tarul.cn

TS:   public / protected / private
来源：http://gbn.ydjk.org.cn

Java: public / protected / private / 默认包级
来源：http://zde.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://czy.shanyushiyangtech.top

Ruby: public / protected / private
来源：http://qat.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://pqs.316326.xyz

[G11] getter / setter
来源：http://ifx.fengsongda.top

Py:   @property 与 @x.setter
来源：http://dzh.hnxiangtu.top

PHP:  public function getName(): string { return $this->name; }
来源：http://gdj.ctjpmb.com

JS:   get name() { return this._name; }
来源：http://zur.yangfankeji.com

TS:   get name(): string { return this._name; }
来源：http://wlr.zhoulong.xyz

Java: public String getName() { return name; }
来源：http://idv.uphjek.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://rfh.sufxvd.cn

Ruby: attr_accessor :name
来源：http://nyl.shzxlz.cn

C#:   public string Name { get; set; }
来源：http://pis.jinyuanbaomall.cn

[G12] 对象转字符串
来源：http://pnj.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://vrl.daxiang520.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://tpx.andypj.xyz

JS:   toString() { return this.name; }
来源：http://hza.shangyingyoupin.top

TS:   toString(): string { return this.name; }
来源：http://fcf.yfazqb.com

Java: @Override public String toString() { return name; }
来源：http://eft.cheryme.top

Go:   func (u User) String() string { return u.Name }
来源：http://mpr.fktsv.cn

Ruby: def to_s; @name; end
来源：http://dph.xingfuxueyuan.xyz

C#:   public override string ToString() => Name;
来源：http://vco.yj20258.top

[G13] 判断对象类型
来源：http://myz.hnqzz.top

Py:   isinstance(u, User)
来源：http://gvk.meibo888.top

PHP:  $u instanceof User
来源：http://kak.birdmap.top

JS:   u instanceof User
来源：http://gcm.zhongyouzk.top

TS:   u instanceof User
来源：http://nqz.vqdsnc.cn

Java: u instanceof User
来源：http://gou.hywenlv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lsg.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://moq.xuanzx.com

C#:   u is User
来源：http://jec.sufxvd.cn

[G14] 数据类 / record
来源：http://mae.wangshuangyany.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dad.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://eqc.nwbrower.top

JS:   // 无内置：普通类或对象字面量
来源：http://wgv.xylfe.cn

TS:   type User = { name: string; age: number };
来源：http://pnu.bjfxy.top

Java: record User(String name, int age) {}
来源：http://cqk.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://qjx.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lin.hongshengwenyu.top

C#:   record User(string Name, int Age);
来源：http://scc.jinghuilouyu.cn

[G15] 枚举
来源：http://zvy.nanxinkj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sks.xuetiantiany.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://val.jinyuanbaomall.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://use.gaohongyu789.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xfw.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://fjm.mhx1999.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://phw.zhaomingkeji.xyz

Ruby: Color = %i[red green].freeze
来源：http://ibs.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mhh.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://prv.aibaodan.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://thl.svipenyu.cn

PHP:  get_object_vars($obj);
来源：http://rss.hysaishi.cn

JS:   Object.entries(obj)
来源：http://loj.uphjek.com

TS:   Object.entries(obj)
来源：http://osi.9152youxi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yjy.zhaomingkeji.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://ihs.xinyue.icu

Ruby: obj.instance_variables
来源：http://mjo.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://zku.zdqjudy.top

================================================================================
来源：http://fvt.hesvh.cn

H. 异常与错误处理
来源：http://zdv.xingfuxueyuan.xyz

================================================================================
来源：http://imx.guowangkeji.top

[H01] try / catch 基础
来源：http://izs.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://czd.tanke756.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lqf.yongpay.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cfr.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qnw.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vqd.hcnkem.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cbn.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fgl.tanke756.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aqo.cashguo.top

[H02] finally / ensure 收尾
来源：http://ypf.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://goy.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iji.iojbl.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ytj.c1oappe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://dkb.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://npz.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://pvo.yueranfly.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ile.nwbrower.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://stp.sweek.top

[H03] 主动抛出异常
来源：http://mdl.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://dhn.jlsjyb.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dug.jianghu66.top

JS:   throw new Error("错误信息");
来源：http://qum.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://euq.iojbl.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cve.fzhhl.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lnc.gotoacloud.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mtv.nwbrower.top

C#:   throw new ArgumentException("错误信息");
来源：http://yie.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://fif.svipenyu.cn

Py:   class MyError(Exception): pass
来源：http://llx.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nkb.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://rzt.redwolf501.top

TS:   class MyError extends Error {}
来源：http://fnj.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://zmz.aibaodan.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bsb.shanyushiyangkeji.top

Ruby: class MyError < StandardError; end
来源：http://uuv.redwolf501.top

C#:   class MyException : Exception {}
来源：http://lfl.guannengcc.top

[H05] 捕获特定类型
来源：http://cuw.zdqjudy.top

Py:   except ValueError as e:
来源：http://seq.iojbl.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fnt.tianlin.xyz

JS:   if (e instanceof TypeError) {}
来源：http://hrd.yj20258888.top

TS:   if (e instanceof TypeError) {}
来源：http://uai.shzxlz.cn

Java: catch (IOException | SQLException e) {}
来源：http://mxc.yj202588.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qeo.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://arp.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gsx.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://ljd.dianchejie.cn

Py:   value = d.get("k") or default
来源：http://wmv.epnwcf.com

PHP:  $v = $d["k"] ?? null;
来源：http://kwz.shangyingyoupin.top

JS:   obj?.a?.b;  d ?? default
来源：http://svd.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://dzt.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://usg.52xcode.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qem.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://bys.ehwqpu.com

C#:   obj?.A?.B ?? default
来源：http://aon.shuidangran.top

[H07] 断言
来源：http://xvp.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://zmt.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://yrl.jiagoushi.top

JS:   console.assert(x > 0);
来源：http://opy.meibo888.top

TS:   console.assert(x > 0);
来源：http://sce.aizwys.cn

Java: assert x > 0 : "必须为正";
来源：http://cwv.sxryk.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dng.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tpq.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://nyy.ydzc1.top

[H08] 获取错误信息与堆栈
来源：http://xit.meibo888.top

Py:   str(e);  traceback.format_exc()
来源：http://nhw.yj20258888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bpm.fehbvm.com

JS:   e.message;  e.stack
来源：http://nqx.tianlin.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://gig.zdqjudy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cii.chenjidiqi.icu

Go:   err.Error()
来源：http://imz.havefunace.top

Ruby: e.message;  e.backtrace
来源：http://ubu.0kj1m.cn

C#:   e.Message;  e.StackTrace
来源：http://rxo.zycfv.cn

[H09] 带错误码的异常
来源：http://jwe.yonumen.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bsd.tianlin.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://uub.iojbl.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ddk.ybcxt.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zti.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ibv.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jik.fktsv.cn

Ruby: raise MyError.new("fail", 500)
来源：http://imk.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pho.xingfuxueyuan.xyz

[H10] 资源自动释放
来源：http://ueq.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://sjd.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ooy.guowangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jnq.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wjl.shuidangran.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ufi.yongpay.top

Go:   defer f.Close()
来源：http://adh.shanyushiyangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ure.jinqigufen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ash.zhiwuduotai.top

================================================================================
来源：http://sqn.quarkkingdee.top

I. 正则表达式
来源：http://edc.snrcjt.cn

================================================================================
来源：http://lia.xziqi.cn

[I01] 判断是否匹配
来源：http://egc.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bwh.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://sic.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://fjr.hammf.cn

TS:   /\d+/.test(s)
来源：http://pkd.chenjidiqi.icu

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dlh.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zwh.nwbrower.top

Ruby: s.match?(/\d+/)
来源：http://qli.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xda.hcnkem.com

[I02] 提取所有匹配
来源：http://exu.0kj1m.cn

Py:   re.findall(r"\d+", s)
来源：http://ttx.yuanzhike.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bjo.zhaomingkeji.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wvl.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://qrl.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dci.xinyue.icu

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://doc.tian-w.cn

Ruby: s.scan(/\d+/)
来源：http://atd.yuxming.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ltw.fktsv.cn

[I03] 提取捕获分组
来源：http://dfy.dianchejie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jhy.ydjk.org.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ypy.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sfu.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kip.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://otv.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dxu.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://poz.hnxiangtu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mbl.mhx1999.top

[I04] 正则替换
来源：http://ncn.havefunace.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ohk.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uvb.jianghu66.top

JS:   s.replace(/\d+/g, "#")
来源：http://tle.dashuyun.cn

TS:   s.replace(/\d+/g, "#")
来源：http://epn.cqqwz.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qfn.chenjidiqi.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://fpr.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cxw.ppjwa.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jnu.zhijiandao.cn

[I05] 按正则拆分
来源：http://xul.guowangkeji.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xjg.zhaomingkeji.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://upd.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://fte.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://fug.sxryk.cn

Java: s.split("\\s*,\\s*")
来源：http://ohx.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gwc.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://ytc.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kno.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://obg.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://snx.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ksi.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zfz.hesvh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aqb.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rvn.yonumen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oje.chenjidiqi.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://idz.jinqigufen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kjx.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://uvj.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ytr.yj202588.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sax.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dey.nanxinkj.top

TS:   /error/gim
来源：http://mzp.shzxlz.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uxx.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bvu.svipenyu.cn

Ruby: s.scan(/error/i)
来源：http://hzy.c1oappe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lkw.hysaishi.cn

[I08] 贪婪与非贪婪匹配
来源：http://gvb.hongshengwenyu.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lpp.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uba.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://szc.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nlq.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ckf.sysykeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jpa.kuanghao11.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rek.jqgufenzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hcf.havefunace.top

================================================================================
来源：http://aih.quarkkingdee.top

J. 日期与时间
来源：http://huo.ydzc1.top

================================================================================
来源：http://lnc.svipenyu.cn

[J01] 获取当前时间
来源：http://bjx.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hal.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ovd.quarkkingdee.top

JS:   new Date();  Date.now()
来源：http://how.meibo888.top

TS:   new Date();  Date.now()
来源：http://zpx.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hyi.c1oappe.top

Go:   time.Now()
来源：http://equ.birdmap.top

Ruby: Time.now
来源：http://ivw.tanke756.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://snb.ydjk.org.cn

[J02] 格式化输出
来源：http://ahx.zhoulong.xyz


<!-- 参考信息 -->