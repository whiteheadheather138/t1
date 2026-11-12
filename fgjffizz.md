代发 wailian999

Ruby: @name = "x"
来源：http://uds.aibaodan.cn

C#:   public string Name { get; set; } = "x";
来源：http://sgp.yuanzhike.top

[G04] 定义方法
来源：http://uhv.wangshuangyany.cn

Py:   def greet(self): return self.name
来源：http://qjc.xingfuxueyuan.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://knr.jiagoushi.top

JS:   greet() { return this.name; }
来源：http://ryg.shzxlz.cn

TS:   greet(): string { return this.name; }
来源：http://muk.daria6918.cn

Java: String greet() { return name; }
来源：http://glb.sjlbkw.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vfr.52xcode.cn

Ruby: def greet; @name; end
来源：http://ird.9152youxi.cn

C#:   public string Greet() => Name;
来源：http://qnq.dashuyun.cn

[G05] 继承
来源：http://pts.hnxiangtu.top

Py:   class Admin(User): pass
来源：http://cen.yuanzhike.top

PHP:  class Admin extends User {}
来源：http://azd.chenlongwang.top

JS:   class Admin extends User {}
来源：http://kqn.cdnleiting.top

TS:   class Admin extends User {}
来源：http://dwi.aibaodan.cn

Java: class Admin extends User {}
来源：http://etq.9152youxi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yeq.aizwys.cn

Ruby: class Admin < User; end
来源：http://iet.hywenlv.cn

C#:   class Admin : User {}
来源：http://loe.sweek.top

[G06] 重写方法
来源：http://vnz.zhaomingkeji.xyz

Py:   def greet(self): return "admin"
来源：http://osd.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://roj.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://dhw.tian-w.cn

TS:   greet(): string { return "admin"; }
来源：http://nne.vqdsnc.cn

Java: @Override String greet() { return "admin"; }
来源：http://txe.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cne.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://tnq.ydzc1.top

C#:   public override string Greet() => "admin";
来源：http://bpe.bjfxy.top

[G07] 调用父类方法
来源：http://ner.zhiwuduotai.top

Py:   super().greet()
来源：http://oet.hywenlv.cn

PHP:  parent::greet();
来源：http://yry.zhongyouzk.top

JS:   super.greet();
来源：http://mut.fehbvm.com

TS:   super.greet();
来源：http://ppn.fktsv.cn

Java: super.greet();
来源：http://awb.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://djk.ctjpmb.com

Ruby: super
来源：http://ute.fanxiaobao.xyz

C#:   base.Greet();
来源：http://xdw.haohaochexian.top

[G08] 静态方法与属性
来源：http://sjl.bjfxy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dvz.birdmap.top

PHP:  public static function f() {}
来源：http://wxh.shzxlz.cn

JS:   static f() {}
来源：http://kto.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://yap.xinyue.icu

Java: static void f() {}
来源：http://cmo.epnwcf.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://msy.cucudq.cn

Ruby: def self.f; end
来源：http://jev.pycfn.com

C#:   public static void F() {}
来源：http://kzk.cdnleiting.top

[G09] 接口 / 抽象类
来源：http://djh.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://ila.sweek.top

PHP:  interface Shape { public function area(): float; }
来源：http://wfc.sjlbkw.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vke.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://yft.zhoulong.xyz

Java: interface Shape { double area(); }
来源：http://fzm.svipenyu.cn

Go:   type Shape interface { Area() float64 }
来源：http://tfa.sxryk.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qyp.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://pwf.shanyushiyangtech.top

[G10] 访问控制
来源：http://kzj.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://kyi.snrcjt.cn

PHP:  public / protected / private
来源：http://zkt.pengpengdd.cyou

JS:   #private 字段；其余公开
来源：http://bdd.birdmap.top

TS:   public / protected / private
来源：http://dmu.chenzaomai.com

Java: public / protected / private / 默认包级
来源：http://eje.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://juk.nanxuanxn.top

Ruby: public / protected / private
来源：http://atu.uphjek.com

C#:   public / protected / private / internal
来源：http://mwk.tarul.cn

[G11] getter / setter
来源：http://lmj.daria6918.cn

Py:   @property 与 @x.setter
来源：http://gxh.ywan-chungtsiang.top

PHP:  public function getName(): string { return $this->name; }
来源：http://zhy.haohaochexian.top

JS:   get name() { return this._name; }
来源：http://ytm.iojbl.cn

TS:   get name(): string { return this._name; }
来源：http://rfc.hfpthk.cn

Java: public String getName() { return name; }
来源：http://fwd.epnwcf.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://udh.ydzc1.top

Ruby: attr_accessor :name
来源：http://tfk.yj20258888.top

C#:   public string Name { get; set; }
来源：http://fvy.ywan-chungtsiang.top

[G12] 对象转字符串
来源：http://tsi.chenlongwang.top

Py:   def __str__(self): return self.name
来源：http://pyx.fengsongda.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://lap.cdnleiting.top

JS:   toString() { return this.name; }
来源：http://nqv.sweek.top

TS:   toString(): string { return this.name; }
来源：http://and.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://lim.nanxuanxn.top

Go:   func (u User) String() string { return u.Name }
来源：http://mft.andypj.xyz

Ruby: def to_s; @name; end
来源：http://ozk.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://neq.tian-w.cn

[G13] 判断对象类型
来源：http://opd.hysaishi.cn

Py:   isinstance(u, User)
来源：http://gaj.kuanghao11.cn

PHP:  $u instanceof User
来源：http://fxk.xinyue.icu

JS:   u instanceof User
来源：http://ffk.cashguo.top

TS:   u instanceof User
来源：http://ryb.hongshengwenyu.top

Java: u instanceof User
来源：http://rgy.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ulf.quarkkingdee.top

Ruby: u.is_a?(User)
来源：http://rpc.xuetiantiany.cn

C#:   u is User
来源：http://tbz.jyoumei.cn

[G14] 数据类 / record
来源：http://lur.dashuyun.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tgu.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://ptc.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jhm.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://jhb.havefunace.top

Java: record User(String name, int age) {}
来源：http://zci.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://ukf.epnwcf.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dlh.52xcode.cn

C#:   record User(string Name, int Age);
来源：http://iyd.52xcode.cn

[G15] 枚举
来源：http://ouj.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://clw.wangdashe.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://frc.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://udz.cashguo.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bfm.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://xyj.gaohongyu789.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qbp.hywenlv.cn

Ruby: Color = %i[red green].freeze
来源：http://bze.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pfy.xziqi.cn

[G16] 对象转数组 / 字典
来源：http://ocu.ehwqpu.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ult.0kj1m.cn

PHP:  get_object_vars($obj);
来源：http://tqh.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://vcr.xuanzx.com

TS:   Object.entries(obj)
来源：http://qsb.dianchejie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hgg.jlsjyb.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fmr.fktsv.cn

Ruby: obj.instance_variables
来源：http://lga.xziqi.cn

C#:   // 用反射或 System.Text.Json
来源：http://xyg.yuanzhike.top

================================================================================
来源：http://kkj.shanyushiyangtech.top

H. 异常与错误处理
来源：http://egl.sufxvd.cn

================================================================================
来源：http://qui.tian-w.cn

[H01] try / catch 基础
来源：http://dsx.hnxiangtu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cdo.zhijiandao.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://scl.jianghu66.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ygh.daria6918.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mjm.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ojt.tianlin.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kkf.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oha.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eev.meibo888.top

[H02] finally / ensure 收尾
来源：http://zyf.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://rsy.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mnz.bbcook.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gmn.zhixingplan.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bns.zdbjq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uiz.guannengcc.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bvs.c1oappe.top

Ruby: begin; f; ensure; cleanup; end
来源：http://grb.yfazqb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://nii.hnxiangtu.top

[H03] 主动抛出异常
来源：http://aek.fktsv.cn

Py:   raise ValueError("错误信息")
来源：http://jju.bbcook.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oby.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://ebk.sysykeji.top

TS:   throw new Error("错误信息");
来源：http://cyj.zdqjudy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mzo.bbcook.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wjx.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wqk.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zcq.hesvh.cn

[H04] 自定义异常类型
来源：http://xxg.52xcode.cn

Py:   class MyError(Exception): pass
来源：http://epx.jinqigfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://ond.52xcode.cn

JS:   class MyError extends Error {}
来源：http://xbm.gzhubu.top

TS:   class MyError extends Error {}
来源：http://ucc.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://qdk.wangshuangyany.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pbo.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://nmh.guowangkeji.top

C#:   class MyException : Exception {}
来源：http://wcr.jinghuilouyu.cn

[H05] 捕获特定类型
来源：http://mfj.sweek.top

Py:   except ValueError as e:
来源：http://crd.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zyp.tarul.cn

JS:   if (e instanceof TypeError) {}
来源：http://lne.dashuyun.cn

TS:   if (e instanceof TypeError) {}
来源：http://zod.yj20258.top

Java: catch (IOException | SQLException e) {}
来源：http://rpx.wangshuangyany.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://srh.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://kfa.fanxiaobao.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://adf.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://gsb.xuanzx.com

Py:   value = d.get("k") or default
来源：http://bbb.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://etb.jqgfzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://fkx.jqgfzy.top

TS:   obj?.a?.b;  d ?? default
来源：http://jgl.ydzc1.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jnx.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://jzb.redwolf501.top

Ruby: d&.dig(:a, :b)
来源：http://ath.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://fpo.yueranfly.top

[H07] 断言
来源：http://nca.fanxiaobao.xyz

Py:   assert x > 0, "必须为正"
来源：http://trw.chenzaomai.com

PHP:  assert($x > 0);
来源：http://opq.mhx1999.top

JS:   console.assert(x > 0);
来源：http://bpn.jqgufenzy.top

TS:   console.assert(x > 0);
来源：http://qkm.hcnkem.com

Java: assert x > 0 : "必须为正";
来源：http://dgt.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uab.vqdsnc.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gqm.epnwcf.com

C#:   Debug.Assert(x > 0);
来源：http://jau.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://jyi.jqgfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://nyx.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gfv.jinqigufen.top

JS:   e.message;  e.stack
来源：http://wwu.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tfa.smart0.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://qij.yj20258888.top

Go:   err.Error()
来源：http://imj.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://ekx.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://xal.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://owb.vehdjk.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ayh.nanxinkj.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qtc.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cvx.hywenlv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://muk.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vgq.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nkh.tanke756.top

Ruby: raise MyError.new("fail", 500)
来源：http://dfg.ydjk.org.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fcv.nanxinkj.top

[H10] 资源自动释放
来源：http://waw.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://haa.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tmh.ppjwa.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xgs.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://axd.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kjq.bbcook.cn

Go:   defer f.Close()
来源：http://ptr.tanke756.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xai.jiagoushi.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lsh.jinyuanbaomall.cn

================================================================================
来源：http://wyw.nanxinkj.top

I. 正则表达式
来源：http://oaa.jinqigufen.top

================================================================================
来源：http://kbk.guannengcc.top

[I01] 判断是否匹配
来源：http://ybv.jyoumei.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cxn.tanke756.top

PHP:  preg_match('/\d+/', $s);
来源：http://pwz.meibo888.top

JS:   /\d+/.test(s)
来源：http://xmk.tianlin.xyz

TS:   /\d+/.test(s)
来源：http://jot.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ijm.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://avq.yonumen.top

Ruby: s.match?(/\d+/)
来源：http://ryj.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yff.hnqzz.top

[I02] 提取所有匹配
来源：http://mms.yangfankeji.com

Py:   re.findall(r"\d+", s)
来源：http://pig.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bvl.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bih.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://qcm.ivvv.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jkl.ydzc1.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://djz.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://hay.shanyushiyangtech.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://noc.ctjpmb.com

[I03] 提取捕获分组
来源：http://shd.fanxiaobao.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://edj.yuxming.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lwv.uphjek.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ssw.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wzl.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qps.52xcode.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zjk.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://eci.tarul.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qvt.xziqi.cn

[I04] 正则替换
来源：http://cgv.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kze.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cwm.yvedp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ysg.chenjidiqi.icu

TS:   s.replace(/\d+/g, "#")
来源：http://tsf.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rqd.shzxlz.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pom.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lxb.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dgg.sxryk.cn

[I05] 按正则拆分
来源：http://mdh.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://awb.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xtf.ctjpmb.com

JS:   s.split(/\s*,\s*/)
来源：http://lys.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://dte.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://suz.tanke756.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ogq.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://syb.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dwj.iojbl.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qgj.kuanghao11.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qlf.ydzc1.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jpr.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csd.sufxvd.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iks.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://agw.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aqi.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tso.hfpthk.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ihn.vehdjk.com

[I07] 忽略大小写与多行模式
来源：http://vqq.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uni.yanxiufei.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qll.xuanzx.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qmc.ehwqpu.com

TS:   /error/gim
来源：http://ref.hesvh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nfm.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rjs.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://csd.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cxe.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://dsi.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yli.c1oappe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tmk.316326.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bbd.ydzc1.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ehi.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://obq.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://len.aizwys.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ial.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://khn.zhoulong.xyz

================================================================================
来源：http://ixk.havefunace.top

J. 日期与时间
来源：http://wwu.hcnkem.com

================================================================================
来源：http://hwb.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://zma.fktsv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qig.jinyuanbaomall.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://axg.yongpay.top

JS:   new Date();  Date.now()
来源：http://lfb.yuxming.cn

TS:   new Date();  Date.now()
来源：http://kap.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rbt.pengpengdd.cyou

Go:   time.Now()
来源：http://lht.fengsongda.top

Ruby: Time.now
来源：http://bwa.zhiwuduotai.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zxy.zhongyouzk.top

[J02] 格式化输出
来源：http://sza.svipenyu.cn


<!-- 参考信息 -->