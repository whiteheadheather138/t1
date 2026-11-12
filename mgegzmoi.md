代发 wailian999

Ruby: super
来源：http://ieq.vehdjk.com

C#:   base.Greet();
来源：http://axy.chenlongwang.top

[G08] 静态方法与属性
来源：http://gue.tianlin.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cbv.smart0.xyz

PHP:  public static function f() {}
来源：http://met.havefunace.top

JS:   static f() {}
来源：http://tvy.epnwcf.com

TS:   static f(): void {}
来源：http://wpn.nwbrower.top

Java: static void f() {}
来源：http://mtn.ydzc1.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kqp.xingfuxueyuan.xyz

Ruby: def self.f; end
来源：http://qxm.chenjidiqi.icu

C#:   public static void F() {}
来源：http://kff.tian-w.cn

[G09] 接口 / 抽象类
来源：http://hji.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://djh.yj202588.top

PHP:  interface Shape { public function area(): float; }
来源：http://wnp.bjfxy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://rvt.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://zgy.cheryme.top

Java: interface Shape { double area(); }
来源：http://nyr.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://wrv.chenjidiqi.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cjo.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://hlo.wangshuangyany.cn

[G10] 访问控制
来源：http://ess.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://mze.tianlin.xyz

PHP:  public / protected / private
来源：http://ovr.nanxuanxn.top

JS:   #private 字段；其余公开
来源：http://ilm.zhixingplan.top

TS:   public / protected / private
来源：http://zko.hongshengwenyu.top

Java: public / protected / private / 默认包级
来源：http://lsa.0kj1m.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gvt.316326.xyz

Ruby: public / protected / private
来源：http://dqf.hysaishi.cn

C#:   public / protected / private / internal
来源：http://jfo.pycfn.com

[G11] getter / setter
来源：http://alk.uphjek.com

Py:   @property 与 @x.setter
来源：http://bms.daxiang520.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hmw.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://kex.ybcxt.top

TS:   get name(): string { return this._name; }
来源：http://ncr.zhongyouzk.top

Java: public String getName() { return name; }
来源：http://pxg.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mev.sjlbkw.cn

Ruby: attr_accessor :name
来源：http://idc.ehwqpu.com

C#:   public string Name { get; set; }
来源：http://wwb.fengsongda.top

[G12] 对象转字符串
来源：http://qsa.52xcode.cn

Py:   def __str__(self): return self.name
来源：http://kip.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://coq.nanxinkj.top

JS:   toString() { return this.name; }
来源：http://iev.wangdashe.top

TS:   toString(): string { return this.name; }
来源：http://wns.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://fpp.hongshengwenyu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ztj.gogol.net.cn

Ruby: def to_s; @name; end
来源：http://qdr.fengsongda.top

C#:   public override string ToString() => Name;
来源：http://lsj.yuanzhike.top

[G13] 判断对象类型
来源：http://qik.gotoacloud.top

Py:   isinstance(u, User)
来源：http://hyp.sweek.top

PHP:  $u instanceof User
来源：http://dor.bbcook.cn

JS:   u instanceof User
来源：http://pbn.ehwqpu.com

TS:   u instanceof User
来源：http://apj.bbcook.cn

Java: u instanceof User
来源：http://axo.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qxy.yanxiufei.cn

Ruby: u.is_a?(User)
来源：http://uey.ctjpmb.com

C#:   u is User
来源：http://iau.fehbvm.com

[G14] 数据类 / record
来源：http://qdp.yongpay.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fwm.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://snk.jqgfzy.top

JS:   // 无内置：普通类或对象字面量
来源：http://oac.hcnkem.com

TS:   type User = { name: string; age: number };
来源：http://jcw.quarkkingdee.top

Java: record User(String name, int age) {}
来源：http://cbw.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://sfe.yonumen.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bqk.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://esj.0kj1m.cn

[G15] 枚举
来源：http://hfs.yuanzhike.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jsc.fehbvm.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://was.wangdashe.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mfm.havefunace.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yvi.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://mxy.sufxvd.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dip.guowangkeji.top

Ruby: Color = %i[red green].freeze
来源：http://msu.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qxk.52xcode.cn

[G16] 对象转数组 / 字典
来源：http://wyt.hnqzz.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://amv.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://dfi.aibaodan.cn

JS:   Object.entries(obj)
来源：http://wsh.jyoumei.cn

TS:   Object.entries(obj)
来源：http://qmb.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ktp.chenlongwang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://iie.bbcook.cn

Ruby: obj.instance_variables
来源：http://ktf.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://tti.sweek.top

================================================================================
来源：http://jih.yfazqb.com

H. 异常与错误处理
来源：http://phl.yj202588.top

================================================================================
来源：http://ddp.zhoulong.xyz

[H01] try / catch 基础
来源：http://uok.zhoulong.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://azd.c1oappe.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aso.wangdashe.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rrd.tianlin.xyz

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cgq.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://snq.hammf.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ogc.feifeiyinyue.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jgl.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ytx.zhongyouzk.top

[H02] finally / ensure 收尾
来源：http://zav.snrcjt.cn

Py:   try: f()⏎finally: cleanup()
来源：http://stp.jqgfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nfy.52xcode.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://frv.wangshuangyany.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kau.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://bsx.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ljk.zdqjudy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ddu.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://tpn.zdbjq.cn

[H03] 主动抛出异常
来源：http://clh.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://jcv.xingfuxueyuan.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mzw.guowangkeji.top

JS:   throw new Error("错误信息");
来源：http://jim.yuxming.cn

TS:   throw new Error("错误信息");
来源：http://fbj.andypj.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://gkj.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ohd.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oky.feifeiyinyue.top

C#:   throw new ArgumentException("错误信息");
来源：http://tga.epnwcf.com

[H04] 自定义异常类型
来源：http://afg.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://jay.sweek.top

PHP:  class MyError extends RuntimeException {}
来源：http://xln.dianchejie.cn

JS:   class MyError extends Error {}
来源：http://cvs.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://cvi.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://qvk.hongshengwenyu.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cye.ivvv.top

Ruby: class MyError < StandardError; end
来源：http://lwh.chenlongwang.top

C#:   class MyException : Exception {}
来源：http://jme.hywenlv.cn

[H05] 捕获特定类型
来源：http://fcg.0kj1m.cn

Py:   except ValueError as e:
来源：http://nce.fanxiaobao.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qkz.fzhhl.top

JS:   if (e instanceof TypeError) {}
来源：http://kmm.ehwqpu.com

TS:   if (e instanceof TypeError) {}
来源：http://gxj.52xcode.cn

Java: catch (IOException | SQLException e) {}
来源：http://pqi.zdqjudy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hkb.redwolf501.top

Ruby: rescue ArgumentError => e
来源：http://lyi.yj202588.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zoy.gotoacloud.top

[H06] 可选值 / 空值安全访问
来源：http://enl.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://opk.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://zlg.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vzg.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://jdt.c1oappe.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pgo.cqqwz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nki.jinqigfzy.top

Ruby: d&.dig(:a, :b)
来源：http://qpz.hammf.cn

C#:   obj?.A?.B ?? default
来源：http://kiu.ydjk.org.cn

[H07] 断言
来源：http://fsi.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://rva.ehwqpu.com

PHP:  assert($x > 0);
来源：http://rap.sxryk.cn

JS:   console.assert(x > 0);
来源：http://xal.tanke756.top

TS:   console.assert(x > 0);
来源：http://iif.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://rgg.zycfv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fhx.jlsjyb.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mrq.shanyushiyangtech.top

C#:   Debug.Assert(x > 0);
来源：http://btg.ybcxt.top

[H08] 获取错误信息与堆栈
来源：http://mvx.chenzaomai.com

Py:   str(e);  traceback.format_exc()
来源：http://wez.daria6918.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bjo.yj20258.top

JS:   e.message;  e.stack
来源：http://zen.jyoumei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://owv.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://gzc.xinyue.icu

Go:   err.Error()
来源：http://brq.nanxuanxn.top

Ruby: e.message;  e.backtrace
来源：http://yes.bjfxy.top

C#:   e.Message;  e.StackTrace
来源：http://ikn.ydjk.org.cn

[H09] 带错误码的异常
来源：http://lvw.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://htu.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wsi.sysykeji.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hld.shanyushiyangtech.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pub.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qeu.shangyingyoupin.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pxg.jqgfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://esu.meibo888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zhr.hesvh.cn

[H10] 资源自动释放
来源：http://plo.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zvy.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ndh.0kj1m.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hrm.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jvz.tarul.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://snn.zhiwuduotai.top

Go:   defer f.Close()
来源：http://wir.zhengqikj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yjh.chenzaomai.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uoe.52xcode.cn

================================================================================
来源：http://lau.jiagoushi.top

I. 正则表达式
来源：http://csg.52xcode.cn

================================================================================
来源：http://xwe.fengsongda.top

[I01] 判断是否匹配
来源：http://kir.tianlin.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pao.shzxlz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hxh.jinghuilouyu.cn

JS:   /\d+/.test(s)
来源：http://qpg.cdnleiting.top

TS:   /\d+/.test(s)
来源：http://wgq.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nbj.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sma.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://qqm.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lvc.smart0.xyz

[I02] 提取所有匹配
来源：http://mim.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://ony.redwolf501.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://sba.vqdsnc.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oen.zhiwuduotai.top

TS:   s.match(/\d+/g)
来源：http://syw.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zob.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://slt.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://wsw.zhijiandao.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bin.zdqjudy.top

[I03] 提取捕获分组
来源：http://uxt.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ead.svipenyu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fco.kuanghao11.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wol.fzhhl.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lxd.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://itt.jqgfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zjk.yfazqb.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zjj.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ysb.shangyingyoupin.top

[I04] 正则替换
来源：http://bnq.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://cnr.zhongyouzk.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vlg.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ddy.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://wyd.xziqi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kmf.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ykt.andypj.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://hdf.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tmi.nwbrower.top

[I05] 按正则拆分
来源：http://qtj.birdmap.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wuh.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://npu.ydzc1.top

JS:   s.split(/\s*,\s*/)
来源：http://rbs.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://vnv.fehbvm.com

Java: s.split("\\s*,\\s*")
来源：http://xlc.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jbw.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ioh.yj20258.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kec.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vuw.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ndj.ppjwa.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hza.wangshuangyany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tjp.yuxming.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cws.yj202588.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jhr.sweek.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ujr.jinqigufen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pgz.guowangkeji.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mxs.zhixingplan.top

[I07] 忽略大小写与多行模式
来源：http://hdk.ywan-chungtsiang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://abi.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hvl.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kln.hongshengwenyu.top

TS:   /error/gim
来源：http://gyf.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qag.hnqzz.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zzq.zhaomingkeji.xyz

Ruby: s.scan(/error/i)
来源：http://rrq.zdqjudy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yne.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://hyo.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xsv.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fmj.52xcode.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfl.aizwys.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hfa.xuanzx.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://lwy.zycfv.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oal.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://koa.fanxiaobao.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://psa.pengpengdd.cyou

================================================================================
来源：http://xcg.jqgufenzy.top

J. 日期与时间
来源：http://ejj.zhoulong.xyz

================================================================================
来源：http://fng.guannengcc.top

[J01] 获取当前时间
来源：http://qlb.ppjwa.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hmj.yueranfly.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://inl.hnqzz.top

JS:   new Date();  Date.now()
来源：http://fcb.zhongyouzk.top

TS:   new Date();  Date.now()
来源：http://wjz.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://omw.nanxinkj.top

Go:   time.Now()
来源：http://pxw.xingfuxueyuan.xyz

Ruby: Time.now
来源：http://zsw.xinyue.icu

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lin.smart0.xyz

[J02] 格式化输出
来源：http://tzv.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kds.aibaodan.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oij.hywenlv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://niq.bbcook.cn

TS:   d.toISOString()
来源：http://abu.pengpengdd.cyou

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zzi.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ggn.9152youxi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mzr.birdmap.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ylm.zdqjudy.top

[J03] 字符串解析为日期
来源：http://lww.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jjf.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kmu.mhx1999.top

JS:   new Date("2024-01-02")
来源：http://wfy.zdqjudy.top

TS:   new Date("2024-01-02")
来源：http://djy.yonumen.top

Java: LocalDate.parse("2024-01-02")
来源：http://yhe.xylfe.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ntk.zhongyouzk.top

Ruby: Date.parse("2024-01-02")
来源：http://mpb.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ddy.jqgufenzy.top

[J04] 时间戳与日期互转
来源：http://tec.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://icf.shanyushiyangtech.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qch.zdqjudy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pzf.ivvv.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vzz.ywan-chungtsiang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jnh.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qnx.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tdb.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://krz.tanke756.top

[J05] 时间加减（加 7 天）
来源：http://hfn.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://rin.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://vza.mhx1999.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ghd.ydzc1.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bet.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://zzg.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wts.aizwys.cn

Ruby: Time.now + 7 * 86400
来源：http://ghu.andypj.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ofj.sweek.top

[J06] 计算两时间之差
来源：http://jcq.jianghu66.top


<!-- 参考信息 -->