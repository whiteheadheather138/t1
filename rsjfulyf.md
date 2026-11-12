代发 wailian999

PHP:  public static function f() {}
来源：http://cql.svipenyu.cn

JS:   static f() {}
来源：http://lob.tian-w.cn

TS:   static f(): void {}
来源：http://iee.ywan-chungtsiang.top

Java: static void f() {}
来源：http://owc.yvedp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ygh.tarul.cn

Ruby: def self.f; end
来源：http://cyk.tarul.cn

C#:   public static void F() {}
来源：http://uef.zhoulong.xyz

[G09] 接口 / 抽象类
来源：http://txh.zdbjq.cn

Py:   from abc import ABC, abstractmethod
来源：http://hsc.c1oappe.top

PHP:  interface Shape { public function area(): float; }
来源：http://kdn.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lju.zhixingplan.top

TS:   interface Shape { area(): number; }
来源：http://klb.bjfxy.top

Java: interface Shape { double area(); }
来源：http://ply.ctjpmb.com

Go:   type Shape interface { Area() float64 }
来源：http://qya.hcnkem.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nco.ydzc1.top

C#:   interface IShape { double Area(); }
来源：http://poc.hnxiangtu.top

[G10] 访问控制
来源：http://lne.snrcjt.cn

Py:   约定 _protected / __private（不强制）
来源：http://fit.hysaishi.cn

PHP:  public / protected / private
来源：http://mcn.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://vtd.hnxiangtu.top

TS:   public / protected / private
来源：http://odn.epnwcf.com

Java: public / protected / private / 默认包级
来源：http://djg.uphjek.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://dkc.yanxiufei.cn

Ruby: public / protected / private
来源：http://vlf.tianlin.xyz

C#:   public / protected / private / internal
来源：http://iem.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://ils.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://uqf.yongpay.top

PHP:  public function getName(): string { return $this->name; }
来源：http://btn.yj202588.top

JS:   get name() { return this._name; }
来源：http://biz.jinqigufen.top

TS:   get name(): string { return this._name; }
来源：http://hpy.yanxiufei.cn

Java: public String getName() { return name; }
来源：http://mil.jqgufenzy.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yky.dianchejie.cn

Ruby: attr_accessor :name
来源：http://gvt.hysaishi.cn

C#:   public string Name { get; set; }
来源：http://dqa.meibo888.top

[G12] 对象转字符串
来源：http://pgx.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://pyo.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zri.sysykeji.top

JS:   toString() { return this.name; }
来源：http://oky.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://ekc.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://pzz.snrcjt.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hxz.sxryk.cn

Ruby: def to_s; @name; end
来源：http://lpa.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://ann.sufxvd.cn

[G13] 判断对象类型
来源：http://mqr.hfpthk.cn

Py:   isinstance(u, User)
来源：http://jgi.pengpengdd.cyou

PHP:  $u instanceof User
来源：http://qcj.zhijiandao.cn

JS:   u instanceof User
来源：http://hcc.birdmap.top

TS:   u instanceof User
来源：http://pxd.cheryme.top

Java: u instanceof User
来源：http://ggi.yuxming.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jpj.hywenlv.cn

Ruby: u.is_a?(User)
来源：http://eoz.fanxiaobao.xyz

C#:   u is User
来源：http://knm.jinghuilouyu.cn

[G14] 数据类 / record
来源：http://hvg.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fov.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://loy.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jav.fengsongda.top

TS:   type User = { name: string; age: number };
来源：http://cpd.fehbvm.com

Java: record User(String name, int age) {}
来源：http://hhe.yanxiufei.cn

Go:   type User struct { Name string; Age int }
来源：http://hcl.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rbi.redwolf501.top

C#:   record User(string Name, int Age);
来源：http://qpm.shanyushiyangtech.top

[G15] 枚举
来源：http://xqo.yongpay.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wzr.ydjk.org.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpc.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fai.yangfankeji.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baw.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://cey.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://krf.iojbl.cn

Ruby: Color = %i[red green].freeze
来源：http://jaq.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qfi.havefunace.top

[G16] 对象转数组 / 字典
来源：http://pan.tianlin.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hvu.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://adf.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://zxx.hammf.cn

TS:   Object.entries(obj)
来源：http://sgr.fehbvm.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gsp.nanxinkj.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://uej.uphjek.com

Ruby: obj.instance_variables
来源：http://dlj.cqqwz.cn

C#:   // 用反射或 System.Text.Json
来源：http://krm.cqqwz.cn

================================================================================
来源：http://lfz.ehwqpu.com

H. 异常与错误处理
来源：http://ukk.hnqzz.top

================================================================================
来源：http://fgm.wangshuangyany.cn

[H01] try / catch 基础
来源：http://aav.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tkn.ydjk.org.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pjp.zhongyouzk.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bvm.chenlongwang.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wnu.havefunace.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://adv.yuxming.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lec.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ukq.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qlt.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://oga.ehwqpu.com

Py:   try: f()⏎finally: cleanup()
来源：http://mka.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ryr.birdmap.top

JS:   try { f(); } finally { cleanup(); }
来源：http://lxj.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gmv.haohaochexian.top

Java: try { f(); } finally { cleanup(); }
来源：http://sdc.mhx1999.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://idj.xziqi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jww.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://rkz.jqgufenzy.top

[H03] 主动抛出异常
来源：http://miu.yuxming.cn

Py:   raise ValueError("错误信息")
来源：http://guk.9152youxi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ktk.birdmap.top

JS:   throw new Error("错误信息");
来源：http://yfb.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://zrk.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fby.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cgg.andypj.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://qxr.jianghu66.top

C#:   throw new ArgumentException("错误信息");
来源：http://sft.nwbrower.top

[H04] 自定义异常类型
来源：http://ipf.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://azg.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dut.yonumen.top

JS:   class MyError extends Error {}
来源：http://mps.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://twd.hnqzz.top

Java: class MyException extends RuntimeException {}
来源：http://uwh.yangfankeji.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mzf.kuanghao11.cn

Ruby: class MyError < StandardError; end
来源：http://qht.zhixingplan.top

C#:   class MyException : Exception {}
来源：http://yqf.fehbvm.com

[H05] 捕获特定类型
来源：http://zht.sufxvd.cn

Py:   except ValueError as e:
来源：http://yxy.aizwys.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zuq.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://bsa.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://pjl.cdnleiting.top

Java: catch (IOException | SQLException e) {}
来源：http://gjv.shangyingyoupin.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://aki.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://qxy.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pck.feifeiyinyue.top

[H06] 可选值 / 空值安全访问
来源：http://hko.ctjpmb.com

Py:   value = d.get("k") or default
来源：http://xgo.yongpay.top

PHP:  $v = $d["k"] ?? null;
来源：http://yyz.yongpay.top

JS:   obj?.a?.b;  d ?? default
来源：http://fre.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zwh.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lit.fanxiaobao.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://ocm.zhengqikj.top

Ruby: d&.dig(:a, :b)
来源：http://rep.xuanzx.com

C#:   obj?.A?.B ?? default
来源：http://vcz.epnwcf.com

[H07] 断言
来源：http://csj.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://uig.jyoumei.cn

PHP:  assert($x > 0);
来源：http://ecr.zhengqikj.top

JS:   console.assert(x > 0);
来源：http://pyr.yanxiufei.cn

TS:   console.assert(x > 0);
来源：http://drq.yfazqb.com

Java: assert x > 0 : "必须为正";
来源：http://txk.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pcb.wangdashe.top

Ruby: raise "必须为正" unless x > 0
来源：http://kdb.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://bma.aizwys.cn

[H08] 获取错误信息与堆栈
来源：http://yqz.zhiwuduotai.top

Py:   str(e);  traceback.format_exc()
来源：http://ous.tian-w.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tty.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://hud.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://bdn.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://usc.ydjk.org.cn

Go:   err.Error()
来源：http://zid.yj20258.top

Ruby: e.message;  e.backtrace
来源：http://eav.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://vcr.guannengcc.top

[H09] 带错误码的异常
来源：http://gre.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mzz.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cuw.cqqwz.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gde.jianghu66.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lhg.svipenyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gir.hysaishi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jmi.dianchejie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pkz.zhongyouzk.top

C#:   // 自定义异常类中加 Code 属性
来源：http://abf.shuidangran.top

[H10] 资源自动释放
来源：http://ypd.xinyue.icu

Py:   with open("a.txt") as f: data = f.read()
来源：http://nms.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sav.pengpengdd.cyou

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pzc.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hty.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://npz.shanyushiyangtech.top

Go:   defer f.Close()
来源：http://tro.xinyue.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ltq.jyoumei.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ueo.tian-w.cn

================================================================================
来源：http://mib.zhaomingkeji.xyz

I. 正则表达式
来源：http://icl.cucudq.cn

================================================================================
来源：http://ujr.xziqi.cn

[I01] 判断是否匹配
来源：http://lbs.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://peu.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://wwu.bjfxy.top

JS:   /\d+/.test(s)
来源：http://fps.316326.xyz

TS:   /\d+/.test(s)
来源：http://pic.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jgh.yfazqb.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iae.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://xyx.hesvh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lkj.redwolf501.top

[I02] 提取所有匹配
来源：http://ndd.fanxiaobao.xyz

Py:   re.findall(r"\d+", s)
来源：http://gsf.svipenyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nba.hammf.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kni.c1oappe.top

TS:   s.match(/\d+/g)
来源：http://vos.yj202588.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lig.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wxl.c1oappe.top

Ruby: s.scan(/\d+/)
来源：http://qbj.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lnk.dashuyun.cn

[I03] 提取捕获分组
来源：http://glw.cqqwz.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://amg.sysykeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gkh.zhoulong.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wzd.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ahu.cucudq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mat.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rwo.haohaochexian.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ksn.dashuyun.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ove.hywenlv.cn

[I04] 正则替换
来源：http://ycr.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aqh.cqqwz.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jbf.shuidangran.top

JS:   s.replace(/\d+/g, "#")
来源：http://fav.vehdjk.com

TS:   s.replace(/\d+/g, "#")
来源：http://dzo.9152youxi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://och.bjfxy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://vjc.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dks.shangyingyoupin.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jfy.andypj.xyz

[I05] 按正则拆分
来源：http://ubf.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://jrb.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://twr.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://moo.yueranfly.top

TS:   s.split(/\s*,\s*/)
来源：http://eci.gzhubu.top

Java: s.split("\\s*,\\s*")
来源：http://jiq.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wot.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eoa.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lez.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://myh.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rmx.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nnq.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iog.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbe.shzxlz.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yzv.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vba.gotoacloud.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://aqt.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fmx.svipenyu.cn

[I07] 忽略大小写与多行模式
来源：http://cog.gzhubu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ckj.chenzaomai.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ckr.daxiang520.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tzq.kuanghao11.cn

TS:   /error/gim
来源：http://efd.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pxd.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xoe.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://ucd.shzxlz.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pft.dashuyun.cn

[I08] 贪婪与非贪婪匹配
来源：http://hti.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://abc.gogol.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wgd.uphjek.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nkk.chenjidiqi.icu

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vpg.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://aco.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hwx.daxiang520.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ckv.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cnt.fzhhl.top

================================================================================
来源：http://mlw.sysykeji.top

J. 日期与时间
来源：http://ltp.zhixingplan.top

================================================================================
来源：http://vhh.xziqi.cn

[J01] 获取当前时间
来源：http://fus.hfpthk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wli.chenlongwang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nob.gzhubu.top

JS:   new Date();  Date.now()
来源：http://see.shangyingyoupin.top

TS:   new Date();  Date.now()
来源：http://gpk.sweek.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ubb.yueranfly.top

Go:   time.Now()
来源：http://ies.zhaomingkeji.xyz

Ruby: Time.now
来源：http://bzs.yueranfly.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zjz.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://wlc.c1oappe.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zet.nanxinkj.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uqe.jlsjyb.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fpm.bjfxy.top

TS:   d.toISOString()
来源：http://dzh.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ius.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://goz.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hbi.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uib.svipenyu.cn

[J03] 字符串解析为日期
来源：http://rju.yfazqb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nuk.hfpthk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cbz.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://hoe.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://ncn.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://brr.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qzt.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://ygh.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cai.fengsongda.top

[J04] 时间戳与日期互转
来源：http://iaq.ehwqpu.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://moy.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://krn.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://olb.xingfuxueyuan.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://cjb.sweek.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lcu.chenjidiqi.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ahz.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://soq.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wlx.feifeiyinyue.top

[J05] 时间加减（加 7 天）
来源：http://jrd.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://doc.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qrq.tanke756.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gqs.yonumen.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zfn.c1oappe.top

Java: LocalDate.now().plusDays(7)
来源：http://bmq.hfpthk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mdu.jinyuanbaomall.cn

Ruby: Time.now + 7 * 86400
来源：http://ihn.aizwys.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mbi.ydjk.org.cn

[J06] 计算两时间之差
来源：http://uzi.yvedp.cn

Py:   (end - start).total_seconds()
来源：http://iva.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://trq.fanxiaobao.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fgz.ywan-chungtsiang.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ifb.meibo888.top


<!-- 参考信息 -->