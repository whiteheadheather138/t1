代发 wailian999

Ruby: super
来源：http://hbg.316326.xyz

C#:   base.Greet();
来源：http://iqn.tianlin.xyz

[G08] 静态方法与属性
来源：http://isu.aibaodan.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://chg.yongpay.top

PHP:  public static function f() {}
来源：http://oua.ydjk.org.cn

JS:   static f() {}
来源：http://ixm.yj20258.top

TS:   static f(): void {}
来源：http://azw.yonumen.top

Java: static void f() {}
来源：http://dfk.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://vee.mhx1999.top

Ruby: def self.f; end
来源：http://tml.yonumen.top

C#:   public static void F() {}
来源：http://jwf.xinyue.icu

[G09] 接口 / 抽象类
来源：http://ubc.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://khd.dianchejie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yiq.havefunace.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://krs.fengsongda.top

TS:   interface Shape { area(): number; }
来源：http://bpu.yongpay.top

Java: interface Shape { double area(); }
来源：http://yfq.snrcjt.cn

Go:   type Shape interface { Area() float64 }
来源：http://mqj.yangfankeji.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kbg.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://mke.ctjpmb.com

[G10] 访问控制
来源：http://pvs.zycfv.cn

Py:   约定 _protected / __private（不强制）
来源：http://wfy.yangfankeji.com

PHP:  public / protected / private
来源：http://svi.yanxiufei.cn

JS:   #private 字段；其余公开
来源：http://vfy.redwolf501.top

TS:   public / protected / private
来源：http://kly.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://fba.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bwn.cqqwz.cn

Ruby: public / protected / private
来源：http://dfq.guannengcc.top

C#:   public / protected / private / internal
来源：http://swv.daria6918.cn

[G11] getter / setter
来源：http://ylv.xinyue.icu

Py:   @property 与 @x.setter
来源：http://frq.feifeiyinyue.top

PHP:  public function getName(): string { return $this->name; }
来源：http://eil.daria6918.cn

JS:   get name() { return this._name; }
来源：http://qfp.sjlbkw.cn

TS:   get name(): string { return this._name; }
来源：http://mvh.chenlongwang.top

Java: public String getName() { return name; }
来源：http://pvw.zhongyouzk.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yag.iojbl.cn

Ruby: attr_accessor :name
来源：http://mlm.bbcook.cn

C#:   public string Name { get; set; }
来源：http://qej.yonumen.top

[G12] 对象转字符串
来源：http://kaj.zhengqikj.top

Py:   def __str__(self): return self.name
来源：http://fdd.tanke756.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xfg.jianghu66.top

JS:   toString() { return this.name; }
来源：http://lqw.jyoumei.cn

TS:   toString(): string { return this.name; }
来源：http://zws.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://sxl.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qrk.snrcjt.cn

Ruby: def to_s; @name; end
来源：http://mue.ywan-chungtsiang.top

C#:   public override string ToString() => Name;
来源：http://jly.shangyingyoupin.top

[G13] 判断对象类型
来源：http://pcr.52xcode.cn

Py:   isinstance(u, User)
来源：http://zjx.chenlongwang.top

PHP:  $u instanceof User
来源：http://igo.xuanzx.com

JS:   u instanceof User
来源：http://aly.zhengqikj.top

TS:   u instanceof User
来源：http://ouv.xingfuxueyuan.xyz

Java: u instanceof User
来源：http://ykx.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://okp.jinqigufen.top

Ruby: u.is_a?(User)
来源：http://rkj.ydzc1.top

C#:   u is User
来源：http://cuw.fengsongda.top

[G14] 数据类 / record
来源：http://gml.hammf.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kwk.sysykeji.top

PHP:  // 用 readonly 属性模拟
来源：http://bns.vehdjk.com

JS:   // 无内置：普通类或对象字面量
来源：http://pfb.mhx1999.top

TS:   type User = { name: string; age: number };
来源：http://qub.guannengcc.top

Java: record User(String name, int age) {}
来源：http://wqi.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://rli.cucudq.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jgh.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://zbg.aibaodan.cn

[G15] 枚举
来源：http://xyl.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jht.tian-w.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uqo.xziqi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://umj.shangyingyoupin.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://puc.nanxuanxn.top

Java: enum Color { RED, GREEN }
来源：http://dra.pycfn.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dnb.shangyingyoupin.top

Ruby: Color = %i[red green].freeze
来源：http://gxy.fanxiaobao.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gpt.tanke756.top

[G16] 对象转数组 / 字典
来源：http://dvt.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tgd.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://ssg.aizwys.cn

JS:   Object.entries(obj)
来源：http://oqp.aibaodan.cn

TS:   Object.entries(obj)
来源：http://ely.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pxd.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ous.jiagoushi.top

Ruby: obj.instance_variables
来源：http://vgb.jqgufenzy.top

C#:   // 用反射或 System.Text.Json
来源：http://dhu.vqdsnc.cn

================================================================================
来源：http://apr.hnxiangtu.top

H. 异常与错误处理
来源：http://hia.gogol.net.cn

================================================================================
来源：http://wcn.wangdashe.top

[H01] try / catch 基础
来源：http://wit.zdbjq.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wjo.jinghuilouyu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jpx.tianlin.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yrh.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://obo.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pct.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fdl.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gvm.wangshuangyany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://igj.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://cfx.zhijiandao.cn

Py:   try: f()⏎finally: cleanup()
来源：http://imo.meibo888.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hji.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://ydd.ivvv.top

TS:   try { f(); } finally { cleanup(); }
来源：http://mhh.fanxiaobao.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://nar.fanxiaobao.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://sfo.hongshengwenyu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xaa.hammf.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xzb.havefunace.top

[H03] 主动抛出异常
来源：http://xjt.wangshuangyany.cn

Py:   raise ValueError("错误信息")
来源：http://dhh.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uij.jinyuanbaomall.cn

JS:   throw new Error("错误信息");
来源：http://vzk.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://bzi.sxryk.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://afx.uphjek.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iqh.52xcode.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zvz.pengpengdd.cyou

C#:   throw new ArgumentException("错误信息");
来源：http://gci.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://qhm.xuanzx.com

Py:   class MyError(Exception): pass
来源：http://dcy.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wpz.jqgufenzy.top

JS:   class MyError extends Error {}
来源：http://jay.redwolf501.top

TS:   class MyError extends Error {}
来源：http://ofn.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://lqz.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qhp.nanxuanxn.top

Ruby: class MyError < StandardError; end
来源：http://uqp.shanyushiyangtech.top

C#:   class MyException : Exception {}
来源：http://eqx.havefunace.top

[H05] 捕获特定类型
来源：http://fwq.shangyingyoupin.top

Py:   except ValueError as e:
来源：http://orh.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zls.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://iii.zhoulong.xyz

TS:   if (e instanceof TypeError) {}
来源：http://hob.daxiang520.top

Java: catch (IOException | SQLException e) {}
来源：http://kna.bjfxy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kmx.dianchejie.cn

Ruby: rescue ArgumentError => e
来源：http://pcc.hammf.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nzs.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://god.meibo888.top

Py:   value = d.get("k") or default
来源：http://qmc.yonumen.top

PHP:  $v = $d["k"] ?? null;
来源：http://kqc.cucudq.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lkk.ybcxt.top

TS:   obj?.a?.b;  d ?? default
来源：http://xry.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wsg.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vjm.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://nnr.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://otg.hfpthk.cn

[H07] 断言
来源：http://rxr.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://exy.quarkkingdee.top

PHP:  assert($x > 0);
来源：http://ocg.hysaishi.cn

JS:   console.assert(x > 0);
来源：http://rvj.gzhubu.top

TS:   console.assert(x > 0);
来源：http://kmq.quarkkingdee.top

Java: assert x > 0 : "必须为正";
来源：http://cpq.ehwqpu.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://knp.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mte.yj20258888.top

C#:   Debug.Assert(x > 0);
来源：http://rsa.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://klh.hammf.cn

Py:   str(e);  traceback.format_exc()
来源：http://qpt.epnwcf.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://map.kuanghao11.cn

JS:   e.message;  e.stack
来源：http://mhs.zhixingplan.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://saa.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://qpm.yj202588.top

Go:   err.Error()
来源：http://epc.jlsjyb.cn

Ruby: e.message;  e.backtrace
来源：http://mhe.jinyuanbaomall.cn

C#:   e.Message;  e.StackTrace
来源：http://gij.feifeiyinyue.top

[H09] 带错误码的异常
来源：http://bpq.ivvv.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jit.jinqigfzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fet.meibo888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://knw.kuanghao11.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cuo.shanyushiyangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dzg.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ajp.gogol.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://byb.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dan.wangshuangyany.cn

[H10] 资源自动释放
来源：http://xss.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://zok.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zan.zycfv.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eel.yfazqb.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yqk.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vov.sysykeji.top

Go:   defer f.Close()
来源：http://pmj.vqdsnc.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lwk.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kjn.zhoulong.xyz

================================================================================
来源：http://zmd.ybcxt.top

I. 正则表达式
来源：http://bmd.c1oappe.top

================================================================================
来源：http://wgh.yj20258888.top

[I01] 判断是否匹配
来源：http://unw.guannengcc.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kgr.cdnleiting.top

PHP:  preg_match('/\d+/', $s);
来源：http://fsl.zycfv.cn

JS:   /\d+/.test(s)
来源：http://xfy.svipenyu.cn

TS:   /\d+/.test(s)
来源：http://hzk.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kmw.cashguo.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kgw.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://dch.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://riz.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://kou.chenjidiqi.icu

Py:   re.findall(r"\d+", s)
来源：http://eac.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wwh.jinqigufen.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xqx.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://cqr.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://smu.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fuz.daxiang520.top

Ruby: s.scan(/\d+/)
来源：http://ynx.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://diq.yvedp.cn

[I03] 提取捕获分组
来源：http://bfc.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wxt.redwolf501.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gtl.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tfy.yonumen.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hxk.0kj1m.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oto.epnwcf.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fmm.jianghu66.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bdu.tanke756.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xzl.epnwcf.com

[I04] 正则替换
来源：http://utb.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vwe.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pvl.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://oug.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://xkm.vehdjk.com

Java: s.replaceAll("\\d+", "#")
来源：http://alg.yvedp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lit.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sbr.jyoumei.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tmd.zdbjq.cn

[I05] 按正则拆分
来源：http://pbc.yanxiufei.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hmx.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kfm.jiagoushi.top

JS:   s.split(/\s*,\s*/)
来源：http://ezq.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://wlg.ybcxt.top

Java: s.split("\\s*,\\s*")
来源：http://ryd.chenzaomai.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qrk.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pom.xuanzx.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zll.yuanzhike.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mtt.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://glz.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nri.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wyx.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fps.hysaishi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rpk.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bvf.shzxlz.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://boc.aibaodan.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hsp.zhiwuduotai.top

[I07] 忽略大小写与多行模式
来源：http://ath.daria6918.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vgx.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lou.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://law.chenjidiqi.icu

TS:   /error/gim
来源：http://ygs.feifeiyinyue.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mjs.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://agu.jinghuilouyu.cn

Ruby: s.scan(/error/i)
来源：http://rlx.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tsm.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://txt.sxryk.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hgd.zhoulong.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://asj.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxt.tarul.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://suw.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://eus.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qfd.yj20258.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kxo.hywenlv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lmg.smart0.xyz

================================================================================
来源：http://yil.jlsjyb.cn

J. 日期与时间
来源：http://hla.sxryk.cn

================================================================================
来源：http://spr.dashuyun.cn

[J01] 获取当前时间
来源：http://ivx.dashuyun.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://geo.smart0.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sfq.yuanzhike.top

JS:   new Date();  Date.now()
来源：http://zqy.uphjek.com

TS:   new Date();  Date.now()
来源：http://aco.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://usf.aizwys.cn

Go:   time.Now()
来源：http://zwj.mhx1999.top

Ruby: Time.now
来源：http://pox.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qrr.sweek.top

[J02] 格式化输出
来源：http://sfw.xziqi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hit.zhijiandao.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jbu.chenzaomai.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nxu.nanxinkj.top

TS:   d.toISOString()
来源：http://prq.redwolf501.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uzo.meibo888.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hno.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sqv.xinyue.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://otv.nwbrower.top

[J03] 字符串解析为日期
来源：http://ser.andypj.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zgx.quarkkingdee.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tvh.tarul.cn

JS:   new Date("2024-01-02")
来源：http://exc.ppjwa.cn

TS:   new Date("2024-01-02")
来源：http://uab.shuidangran.top

Java: LocalDate.parse("2024-01-02")
来源：http://fsl.birdmap.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qvj.52xcode.cn

Ruby: Date.parse("2024-01-02")
来源：http://eoe.gogol.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rxd.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://nvm.fehbvm.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fwp.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tmn.vehdjk.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pgv.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://wth.yj202588.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rgx.shanyushiyangtech.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eel.yonumen.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zot.shuidangran.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nug.hnxiangtu.top

[J05] 时间加减（加 7 天）
来源：http://jbc.zycfv.cn

Py:   now + timedelta(days=7)
来源：http://mqi.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://loz.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bsg.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://afp.sweek.top

Java: LocalDate.now().plusDays(7)
来源：http://raa.sufxvd.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mwp.ehwqpu.com

Ruby: Time.now + 7 * 86400
来源：http://mne.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://fko.gaohongyu789.top

[J06] 计算两时间之差
来源：http://hld.cheryme.top


<!-- 参考信息 -->