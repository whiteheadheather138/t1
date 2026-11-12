代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://riq.hcnkem.com

Java: @Override String greet() { return "admin"; }
来源：http://ttc.cdnleiting.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mes.xziqi.cn

Ruby: def greet; "admin"; end
来源：http://zad.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://xvs.sjlbkw.cn

[G07] 调用父类方法
来源：http://vud.zhengqikj.top

Py:   super().greet()
来源：http://mdp.aibaodan.cn

PHP:  parent::greet();
来源：http://iyr.ywan-chungtsiang.top

JS:   super.greet();
来源：http://elo.jinyuanbaomall.cn

TS:   super.greet();
来源：http://edz.svipenyu.cn

Java: super.greet();
来源：http://tiw.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jmd.jiagoushi.top

Ruby: super
来源：http://pxt.mhx1999.top

C#:   base.Greet();
来源：http://shq.zdqjudy.top

[G08] 静态方法与属性
来源：http://txh.316326.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tgb.sxryk.cn

PHP:  public static function f() {}
来源：http://wxr.xuetiantiany.cn

JS:   static f() {}
来源：http://dgs.hysaishi.cn

TS:   static f(): void {}
来源：http://jak.yanxiufei.cn

Java: static void f() {}
来源：http://wbt.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://xed.shuidangran.top

Ruby: def self.f; end
来源：http://hbw.snrcjt.cn

C#:   public static void F() {}
来源：http://boz.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://wyv.hammf.cn

Py:   from abc import ABC, abstractmethod
来源：http://ark.jlsjyb.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ity.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://ujy.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://bpu.epnwcf.com

Java: interface Shape { double area(); }
来源：http://ruh.meibo888.top

Go:   type Shape interface { Area() float64 }
来源：http://zjo.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qdh.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://ghl.tanke756.top

[G10] 访问控制
来源：http://nfz.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://nji.hesvh.cn

PHP:  public / protected / private
来源：http://gft.ybcxt.top

JS:   #private 字段；其余公开
来源：http://zzb.smart0.xyz

TS:   public / protected / private
来源：http://dih.yfazqb.com

Java: public / protected / private / 默认包级
来源：http://oaa.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://zhi.hongshengwenyu.top

Ruby: public / protected / private
来源：http://puv.jiagoushi.top

C#:   public / protected / private / internal
来源：http://vot.cucudq.cn

[G11] getter / setter
来源：http://gha.hnxiangtu.top

Py:   @property 与 @x.setter
来源：http://wca.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zyt.zycfv.cn

JS:   get name() { return this._name; }
来源：http://snd.shuidangran.top

TS:   get name(): string { return this._name; }
来源：http://ohm.havefunace.top

Java: public String getName() { return name; }
来源：http://uot.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ueo.ydjk.org.cn

Ruby: attr_accessor :name
来源：http://vif.zhiwuduotai.top

C#:   public string Name { get; set; }
来源：http://obk.jiagoushi.top

[G12] 对象转字符串
来源：http://hrg.cucudq.cn

Py:   def __str__(self): return self.name
来源：http://zwa.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://gty.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://mas.chenzaomai.com

TS:   toString(): string { return this.name; }
来源：http://mor.sjlbkw.cn

Java: @Override public String toString() { return name; }
来源：http://rge.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://tsr.yvedp.cn

Ruby: def to_s; @name; end
来源：http://upl.cqqwz.cn

C#:   public override string ToString() => Name;
来源：http://nuo.vqdsnc.cn

[G13] 判断对象类型
来源：http://wcy.pycfn.com

Py:   isinstance(u, User)
来源：http://jcf.yvedp.cn

PHP:  $u instanceof User
来源：http://vjn.meibo888.top

JS:   u instanceof User
来源：http://qey.fanxiaobao.xyz

TS:   u instanceof User
来源：http://noy.dashuyun.cn

Java: u instanceof User
来源：http://qko.tarul.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ufw.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://azt.yongpay.top

C#:   u is User
来源：http://myv.pycfn.com

[G14] 数据类 / record
来源：http://znw.cqqwz.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dtr.chenzaomai.com

PHP:  // 用 readonly 属性模拟
来源：http://uyz.daxiang520.top

JS:   // 无内置：普通类或对象字面量
来源：http://ngu.xuanzx.com

TS:   type User = { name: string; age: number };
来源：http://zky.jianghu66.top

Java: record User(String name, int age) {}
来源：http://zie.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://dnb.pycfn.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xsk.shuidangran.top

C#:   record User(string Name, int Age);
来源：http://wjd.kuanghao11.cn

[G15] 枚举
来源：http://swp.zdqjudy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nsf.zhaomingkeji.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://lgq.wangshuangyany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rlp.fktsv.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://amf.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://kjd.guowangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://isn.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://dqb.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kci.gogol.net.cn

[G16] 对象转数组 / 字典
来源：http://jna.sufxvd.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mql.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://wxv.fktsv.cn

JS:   Object.entries(obj)
来源：http://teg.snrcjt.cn

TS:   Object.entries(obj)
来源：http://nxt.jinqigfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cfq.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://pki.9152youxi.cn

Ruby: obj.instance_variables
来源：http://vrt.aibaodan.cn

C#:   // 用反射或 System.Text.Json
来源：http://ren.jlsjyb.cn

================================================================================
来源：http://eds.fanxiaobao.xyz

H. 异常与错误处理
来源：http://pmb.wangshuangyany.cn

================================================================================
来源：http://med.hesvh.cn

[H01] try / catch 基础
来源：http://lcu.zhaomingkeji.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://htt.andypj.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://chw.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://euc.jiagoushi.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://biz.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rxg.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mjz.yj20258.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mzo.yj202588.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qgb.316326.xyz

[H02] finally / ensure 收尾
来源：http://uzl.chenjidiqi.icu

Py:   try: f()⏎finally: cleanup()
来源：http://igo.zdbjq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bgd.0kj1m.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vah.tanke756.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hre.hnxiangtu.top

Java: try { f(); } finally { cleanup(); }
来源：http://znn.yfazqb.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://aij.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://pzs.xylfe.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yck.hysaishi.cn

[H03] 主动抛出异常
来源：http://txj.aizwys.cn

Py:   raise ValueError("错误信息")
来源：http://vcm.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cuj.pengpengdd.cyou

JS:   throw new Error("错误信息");
来源：http://sop.hcnkem.com

TS:   throw new Error("错误信息");
来源：http://ffi.chenlongwang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mps.cqqwz.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gyi.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pav.xuanzx.com

C#:   throw new ArgumentException("错误信息");
来源：http://nms.shanyushiyangtech.top

[H04] 自定义异常类型
来源：http://znz.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://ppv.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://hzh.yanxiufei.cn

JS:   class MyError extends Error {}
来源：http://hvb.xingfuxueyuan.xyz

TS:   class MyError extends Error {}
来源：http://pfl.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://fwc.bjfxy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iew.ywan-chungtsiang.top

Ruby: class MyError < StandardError; end
来源：http://mff.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://frm.chenzaomai.com

[H05] 捕获特定类型
来源：http://hza.ydzc1.top

Py:   except ValueError as e:
来源：http://ijt.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://inv.hywenlv.cn

JS:   if (e instanceof TypeError) {}
来源：http://nhu.yangfankeji.com

TS:   if (e instanceof TypeError) {}
来源：http://vxd.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://mna.bbcook.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mcg.hnqzz.top

Ruby: rescue ArgumentError => e
来源：http://vey.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://atw.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://voz.yj20258888.top

Py:   value = d.get("k") or default
来源：http://bbb.gogol.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nxi.yj20258.top

JS:   obj?.a?.b;  d ?? default
来源：http://yug.zycfv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vig.feifeiyinyue.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fpm.shanyushiyangkeji.top

Go:   if v, ok := m["k"]; ok { }
来源：http://hrt.kuanghao11.cn

Ruby: d&.dig(:a, :b)
来源：http://yjm.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://uey.hysaishi.cn

[H07] 断言
来源：http://onj.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://qjn.gzhubu.top

PHP:  assert($x > 0);
来源：http://yyz.chenzaomai.com

JS:   console.assert(x > 0);
来源：http://hnu.dianchejie.cn

TS:   console.assert(x > 0);
来源：http://fnf.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://ouh.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tiq.yueranfly.top

Ruby: raise "必须为正" unless x > 0
来源：http://mpy.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://bcf.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://rxr.yuxming.cn

Py:   str(e);  traceback.format_exc()
来源：http://sdg.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://smr.zdbjq.cn

JS:   e.message;  e.stack
来源：http://yzt.zhongyouzk.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iad.ybcxt.top

Java: e.getMessage();  e.printStackTrace()
来源：http://gxm.haohaochexian.top

Go:   err.Error()
来源：http://afw.bbcook.cn

Ruby: e.message;  e.backtrace
来源：http://uju.jqgfzy.top

C#:   e.Message;  e.StackTrace
来源：http://vxh.chenlongwang.top

[H09] 带错误码的异常
来源：http://moz.jiagoushi.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://def.jinyuanbaomall.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jgl.jiagoushi.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://huj.zhongyouzk.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wjy.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lcm.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pim.bbcook.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hxx.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ive.cdnleiting.top

[H10] 资源自动释放
来源：http://gvi.jqgufenzy.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://taf.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xhh.cheryme.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hyk.cdnleiting.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bla.jqgfzy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://djk.xuetiantiany.cn

Go:   defer f.Close()
来源：http://jlr.uphjek.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ahp.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aqi.sysykeji.top

================================================================================
来源：http://qwm.smart0.xyz

I. 正则表达式
来源：http://kyx.yj202588.top

================================================================================
来源：http://ukf.xylfe.cn

[I01] 判断是否匹配
来源：http://gjd.zycfv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fnb.feifeiyinyue.top

PHP:  preg_match('/\d+/', $s);
来源：http://bew.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://eft.hesvh.cn

TS:   /\d+/.test(s)
来源：http://otm.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pzp.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://val.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://vxi.hnxiangtu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xvt.hnxiangtu.top

[I02] 提取所有匹配
来源：http://dry.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://pbv.wangshuangyany.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rfa.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jpe.mhx1999.top

TS:   s.match(/\d+/g)
来源：http://bwm.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wdy.dashuyun.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://atp.hammf.cn

Ruby: s.scan(/\d+/)
来源：http://koe.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ysx.shuidangran.top

[I03] 提取捕获分组
来源：http://adt.yj20258.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gsp.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lku.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kzv.tianlin.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bvg.meibo888.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rkn.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lbr.yj20258888.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kax.cqqwz.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rxr.xinyue.icu

[I04] 正则替换
来源：http://sse.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vyc.hysaishi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yqn.ppjwa.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ddh.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://pbw.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jcf.yuanzhike.top

Go:   re.ReplaceAllString(s, "#")
来源：http://arb.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ojt.xinyue.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://igz.chenzaomai.com

[I05] 按正则拆分
来源：http://rka.xingfuxueyuan.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://zhx.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ghd.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://vxa.mhx1999.top

TS:   s.split(/\s*,\s*/)
来源：http://khc.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://ykl.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ebp.aibaodan.cn

Ruby: s.split(/\s*,\s*/)
来源：http://glr.svipenyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xyc.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://brj.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yom.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ven.vqdsnc.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yml.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iey.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xtu.zdbjq.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fin.jianghu66.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eqy.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nfs.xuanzx.com

[I07] 忽略大小写与多行模式
来源：http://axe.hammf.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yjj.zhoulong.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mit.tanke756.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://opu.nanxuanxn.top

TS:   /error/gim
来源：http://qmb.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yff.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jpj.fzhhl.top

Ruby: s.scan(/error/i)
来源：http://bcn.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gkh.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://ska.shangyingyoupin.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://omq.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vmn.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mwp.shuidangran.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hzu.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ylx.hesvh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uhk.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oyr.aizwys.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rfj.guannengcc.top

================================================================================
来源：http://qot.ehwqpu.com

J. 日期与时间
来源：http://ejm.hcnkem.com

================================================================================
来源：http://rxy.tianlin.xyz

[J01] 获取当前时间
来源：http://smp.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zxd.daxiang520.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qtb.zhijiandao.cn

JS:   new Date();  Date.now()
来源：http://buj.jianghu66.top

TS:   new Date();  Date.now()
来源：http://wud.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://noy.zdqjudy.top

Go:   time.Now()
来源：http://bmh.jinqigfzy.top

Ruby: Time.now
来源：http://hah.yangfankeji.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qyv.chenlongwang.top

[J02] 格式化输出
来源：http://pex.yongpay.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wjt.yj202588.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wkx.jyoumei.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yoq.jinqigufen.top

TS:   d.toISOString()
来源：http://zza.hongshengwenyu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ykx.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ybf.zhixingplan.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hyl.pycfn.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uzz.yongpay.top

[J03] 字符串解析为日期
来源：http://vpv.aizwys.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jgn.zhongyouzk.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bso.yangfankeji.com

JS:   new Date("2024-01-02")
来源：http://vyn.ybcxt.top

TS:   new Date("2024-01-02")
来源：http://qmp.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://igx.sxryk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rft.sysykeji.top

Ruby: Date.parse("2024-01-02")
来源：http://deh.gzhubu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tuf.chenlongwang.top

[J04] 时间戳与日期互转
来源：http://fsn.hysaishi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bju.ybcxt.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lkq.tianlin.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yhi.cdnleiting.top

TS:   Math.floor(Date.now() / 1000)
来源：http://lss.cheryme.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gko.zhiwuduotai.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xxr.sufxvd.cn


<!-- 参考信息 -->