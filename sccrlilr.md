代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://ema.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://fru.bjfxy.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qob.daxiang520.top

Ruby: def greet; "admin"; end
来源：http://hah.sufxvd.cn

C#:   public override string Greet() => "admin";
来源：http://zah.sweek.top

[G07] 调用父类方法
来源：http://avd.xingfuxueyuan.xyz

Py:   super().greet()
来源：http://qav.uphjek.com

PHP:  parent::greet();
来源：http://fog.nwbrower.top

JS:   super.greet();
来源：http://wqr.sxryk.cn

TS:   super.greet();
来源：http://giz.shuidangran.top

Java: super.greet();
来源：http://abq.hfpthk.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hgb.redwolf501.top

Ruby: super
来源：http://hhj.fehbvm.com

C#:   base.Greet();
来源：http://riz.hcnkem.com

[G08] 静态方法与属性
来源：http://leh.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yii.aizwys.cn

PHP:  public static function f() {}
来源：http://bul.uphjek.com

JS:   static f() {}
来源：http://yqe.sxryk.cn

TS:   static f(): void {}
来源：http://gar.sxryk.cn

Java: static void f() {}
来源：http://viw.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://len.yanxiufei.cn

Ruby: def self.f; end
来源：http://qte.pengpengdd.cyou

C#:   public static void F() {}
来源：http://azt.0kj1m.cn

[G09] 接口 / 抽象类
来源：http://yjl.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://ero.hysaishi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bah.hywenlv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jkc.dashuyun.cn

TS:   interface Shape { area(): number; }
来源：http://zkf.quarkkingdee.top

Java: interface Shape { double area(); }
来源：http://nbe.jyoumei.cn

Go:   type Shape interface { Area() float64 }
来源：http://aem.52xcode.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nkw.hammf.cn

C#:   interface IShape { double Area(); }
来源：http://xqz.xingfuxueyuan.xyz

[G10] 访问控制
来源：http://jpg.sjlbkw.cn

Py:   约定 _protected / __private（不强制）
来源：http://iyl.feifeiyinyue.top

PHP:  public / protected / private
来源：http://tcc.gotoacloud.top

JS:   #private 字段；其余公开
来源：http://rai.shangyingyoupin.top

TS:   public / protected / private
来源：http://plx.sufxvd.cn

Java: public / protected / private / 默认包级
来源：http://iat.zhengqikj.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ugo.nanxinkj.top

Ruby: public / protected / private
来源：http://hfq.smart0.xyz

C#:   public / protected / private / internal
来源：http://fyk.yfazqb.com

[G11] getter / setter
来源：http://how.gotoacloud.top

Py:   @property 与 @x.setter
来源：http://wmi.jiagoushi.top

PHP:  public function getName(): string { return $this->name; }
来源：http://odk.wangdashe.top

JS:   get name() { return this._name; }
来源：http://ouv.zhoulong.xyz

TS:   get name(): string { return this._name; }
来源：http://ume.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://vso.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kin.epnwcf.com

Ruby: attr_accessor :name
来源：http://eub.xylfe.cn

C#:   public string Name { get; set; }
来源：http://wkb.cucudq.cn

[G12] 对象转字符串
来源：http://mlg.havefunace.top

Py:   def __str__(self): return self.name
来源：http://nvg.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ypz.daxiang520.top

JS:   toString() { return this.name; }
来源：http://hst.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://dgk.daxiang520.top

Java: @Override public String toString() { return name; }
来源：http://jkq.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://ldw.yj202588.top

Ruby: def to_s; @name; end
来源：http://mxi.chenzaomai.com

C#:   public override string ToString() => Name;
来源：http://nni.hongshengwenyu.top

[G13] 判断对象类型
来源：http://kol.aibaodan.cn

Py:   isinstance(u, User)
来源：http://spk.aizwys.cn

PHP:  $u instanceof User
来源：http://mvg.guowangkeji.top

JS:   u instanceof User
来源：http://mbh.shzxlz.cn

TS:   u instanceof User
来源：http://rrr.9152youxi.cn

Java: u instanceof User
来源：http://cza.ydjk.org.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://per.shangyingyoupin.top

Ruby: u.is_a?(User)
来源：http://jtt.cqqwz.cn

C#:   u is User
来源：http://vzy.birdmap.top

[G14] 数据类 / record
来源：http://rpu.iojbl.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://owh.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://xhk.zycfv.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tpv.bjfxy.top

TS:   type User = { name: string; age: number };
来源：http://tyf.hywenlv.cn

Java: record User(String name, int age) {}
来源：http://gyc.daria6918.cn

Go:   type User struct { Name string; Age int }
来源：http://yjy.daria6918.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lsc.ywan-chungtsiang.top

C#:   record User(string Name, int Age);
来源：http://kyj.hnxiangtu.top

[G15] 枚举
来源：http://wvr.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ymp.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ief.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hdo.guannengcc.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bds.yj202588.top

Java: enum Color { RED, GREEN }
来源：http://jws.chenjidiqi.icu

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rgp.zhixingplan.top

Ruby: Color = %i[red green].freeze
来源：http://jem.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oru.sjlbkw.cn

[G16] 对象转数组 / 字典
来源：http://zrg.guannengcc.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://byc.hywenlv.cn

PHP:  get_object_vars($obj);
来源：http://esy.gzhubu.top

JS:   Object.entries(obj)
来源：http://kpd.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://pbq.xziqi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://opt.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://vdf.ybcxt.top

Ruby: obj.instance_variables
来源：http://fja.ctjpmb.com

C#:   // 用反射或 System.Text.Json
来源：http://gke.zhijiandao.cn

================================================================================
来源：http://jze.jqgfzy.top

H. 异常与错误处理
来源：http://vbw.yuxming.cn

================================================================================
来源：http://ltq.yj202588.top

[H01] try / catch 基础
来源：http://adj.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vre.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://twg.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jem.fzhhl.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yje.jianghu66.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uso.guannengcc.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cqa.pengpengdd.cyou

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://koi.tian-w.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xwv.zycfv.cn

[H02] finally / ensure 收尾
来源：http://tlc.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://hst.cdnleiting.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://cub.hesvh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://prq.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://czf.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://sou.tian-w.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pes.snrcjt.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nkj.hcnkem.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://gey.meibo888.top

[H03] 主动抛出异常
来源：http://eww.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://zyp.guowangkeji.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mpo.jiagoushi.top

JS:   throw new Error("错误信息");
来源：http://bxs.hnxiangtu.top

TS:   throw new Error("错误信息");
来源：http://puy.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://alt.svipenyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://btr.cucudq.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rmw.cdnleiting.top

C#:   throw new ArgumentException("错误信息");
来源：http://zew.yueranfly.top

[H04] 自定义异常类型
来源：http://vws.hammf.cn

Py:   class MyError(Exception): pass
来源：http://hze.zdbjq.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fws.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://npy.hesvh.cn

TS:   class MyError extends Error {}
来源：http://guv.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://xio.yuanzhike.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rji.yanxiufei.cn

Ruby: class MyError < StandardError; end
来源：http://bkj.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://qfi.ppjwa.cn

[H05] 捕获特定类型
来源：http://qiw.zhixingplan.top

Py:   except ValueError as e:
来源：http://lra.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pxh.c1oappe.top

JS:   if (e instanceof TypeError) {}
来源：http://fwk.ydjk.org.cn

TS:   if (e instanceof TypeError) {}
来源：http://peo.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://psc.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xnm.quarkkingdee.top

Ruby: rescue ArgumentError => e
来源：http://vjn.hfpthk.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://klt.andypj.xyz

[H06] 可选值 / 空值安全访问
来源：http://ska.ehwqpu.com

Py:   value = d.get("k") or default
来源：http://sdk.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ylc.jianghu66.top

JS:   obj?.a?.b;  d ?? default
来源：http://qho.tarul.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qeo.52xcode.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kks.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yvz.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://sja.aibaodan.cn

C#:   obj?.A?.B ?? default
来源：http://iaa.jqgfzy.top

[H07] 断言
来源：http://fqn.fengsongda.top

Py:   assert x > 0, "必须为正"
来源：http://tcp.guannengcc.top

PHP:  assert($x > 0);
来源：http://iyh.fehbvm.com

JS:   console.assert(x > 0);
来源：http://azz.shanyushiyangtech.top

TS:   console.assert(x > 0);
来源：http://dfe.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://xlt.ctjpmb.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eia.yongpay.top

Ruby: raise "必须为正" unless x > 0
来源：http://ljt.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://hpv.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://jby.ctjpmb.com

Py:   str(e);  traceback.format_exc()
来源：http://qqt.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://epk.jyoumei.cn

JS:   e.message;  e.stack
来源：http://dvb.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://req.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://urg.shuidangran.top

Go:   err.Error()
来源：http://cxc.gaohongyu789.top

Ruby: e.message;  e.backtrace
来源：http://qli.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://fgz.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://bus.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gam.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://plo.yonumen.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rvr.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vbm.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xdi.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xek.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fqi.jqgfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fii.zhijiandao.cn

[H10] 资源自动释放
来源：http://qen.xingfuxueyuan.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://cnf.shanyushiyangtech.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://moq.iojbl.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ldt.jyoumei.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gkz.epnwcf.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fng.0kj1m.cn

Go:   defer f.Close()
来源：http://azv.fanxiaobao.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nwo.wangshuangyany.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://elo.jinqigufen.top

================================================================================
来源：http://bjc.316326.xyz

I. 正则表达式
来源：http://uys.gogol.net.cn

================================================================================
来源：http://qbv.jlsjyb.cn

[I01] 判断是否匹配
来源：http://krf.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bhv.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://dve.nanxuanxn.top

JS:   /\d+/.test(s)
来源：http://lpk.gaohongyu789.top

TS:   /\d+/.test(s)
来源：http://pmj.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xyt.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jde.smart0.xyz

Ruby: s.match?(/\d+/)
来源：http://hin.ctjpmb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zvp.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://mqd.ehwqpu.com

Py:   re.findall(r"\d+", s)
来源：http://bap.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yxk.vehdjk.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ejh.bjfxy.top

TS:   s.match(/\d+/g)
来源：http://izb.xinyue.icu

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ofp.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wez.aibaodan.cn

Ruby: s.scan(/\d+/)
来源：http://gpu.quarkkingdee.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tey.iojbl.cn

[I03] 提取捕获分组
来源：http://xnw.hywenlv.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jel.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cag.ehwqpu.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uix.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qpa.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qog.hesvh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xfa.tanke756.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tut.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rww.shanyushiyangkeji.top

[I04] 正则替换
来源：http://ezl.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://stx.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mvh.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://zmj.fehbvm.com

TS:   s.replace(/\d+/g, "#")
来源：http://mxc.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eth.hongshengwenyu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dyh.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://qes.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vws.yvedp.cn

[I05] 按正则拆分
来源：http://kwf.nwbrower.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kbi.sysykeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rlr.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://ruu.hesvh.cn

TS:   s.split(/\s*,\s*/)
来源：http://wlb.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://cpo.ehwqpu.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ihg.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ifj.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jbk.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kuv.gzhubu.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vqd.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gey.ywan-chungtsiang.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rbk.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sov.zdqjudy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ans.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uuj.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cic.tanke756.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hwx.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://ojd.tian-w.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zne.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qgi.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fhp.andypj.xyz

TS:   /error/gim
来源：http://vno.hywenlv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gbp.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jba.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://cdf.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kvs.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://cxs.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ced.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aqx.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vfm.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pzu.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xyy.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uhe.ehwqpu.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://odp.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xju.epnwcf.com

================================================================================
来源：http://cec.gotoacloud.top

J. 日期与时间
来源：http://tkg.chenjidiqi.icu

================================================================================
来源：http://ckh.0kj1m.cn

[J01] 获取当前时间
来源：http://qvi.jianghu66.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fzj.jinqigfzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ynw.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://imv.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://twu.xinyue.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://qgo.c1oappe.top

Go:   time.Now()
来源：http://hzx.zhoulong.xyz

Ruby: Time.now
来源：http://xpg.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jcw.kuanghao11.cn

[J02] 格式化输出
来源：http://ewb.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yuc.uphjek.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bna.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ypv.vqdsnc.cn

TS:   d.toISOString()
来源：http://rcw.ydjk.org.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qfq.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uqo.nanxinkj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rps.hywenlv.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yos.xuetiantiany.cn

[J03] 字符串解析为日期
来源：http://jli.xylfe.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://otn.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ypf.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://fgv.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://cbd.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ykv.cqqwz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zcs.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://fqv.jinyuanbaomall.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dia.jinyuanbaomall.cn

[J04] 时间戳与日期互转
来源：http://lqq.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wqb.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qlp.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hgw.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://oqz.tarul.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nfy.pengpengdd.cyou

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rup.zhongyouzk.top


<!-- 参考信息 -->