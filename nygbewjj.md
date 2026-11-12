代发 wailian999

PHP:  public static function f() {}
来源：http://yvl.bjfxy.top

JS:   static f() {}
来源：http://tmq.uphjek.com

TS:   static f(): void {}
来源：http://scr.ybcxt.top

Java: static void f() {}
来源：http://wlv.yueranfly.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jij.mhx1999.top

Ruby: def self.f; end
来源：http://nmx.shanyushiyangtech.top

C#:   public static void F() {}
来源：http://tkg.wangdashe.top

[G09] 接口 / 抽象类
来源：http://apt.zhongyouzk.top

Py:   from abc import ABC, abstractmethod
来源：http://mri.guannengcc.top

PHP:  interface Shape { public function area(): float; }
来源：http://uts.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ssx.ydjk.org.cn

TS:   interface Shape { area(): number; }
来源：http://hfp.hammf.cn

Java: interface Shape { double area(); }
来源：http://axz.daria6918.cn

Go:   type Shape interface { Area() float64 }
来源：http://rvg.jlsjyb.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wce.sufxvd.cn

C#:   interface IShape { double Area(); }
来源：http://puu.fehbvm.com

[G10] 访问控制
来源：http://rjr.vehdjk.com

Py:   约定 _protected / __private（不强制）
来源：http://szn.fzhhl.top

PHP:  public / protected / private
来源：http://jrl.vqdsnc.cn

JS:   #private 字段；其余公开
来源：http://erh.fengsongda.top

TS:   public / protected / private
来源：http://tkd.quarkkingdee.top

Java: public / protected / private / 默认包级
来源：http://chw.sysykeji.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://fak.uphjek.com

Ruby: public / protected / private
来源：http://vsl.shzxlz.cn

C#:   public / protected / private / internal
来源：http://ifc.wangdashe.top

[G11] getter / setter
来源：http://qtt.redwolf501.top

Py:   @property 与 @x.setter
来源：http://oew.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qdl.fengsongda.top

JS:   get name() { return this._name; }
来源：http://ytd.cashguo.top

TS:   get name(): string { return this._name; }
来源：http://tnc.hywenlv.cn

Java: public String getName() { return name; }
来源：http://vhb.c1oappe.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xbe.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://rom.ppjwa.cn

C#:   public string Name { get; set; }
来源：http://vsx.hcnkem.com

[G12] 对象转字符串
来源：http://bfz.aibaodan.cn

Py:   def __str__(self): return self.name
来源：http://fok.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wvv.yueranfly.top

JS:   toString() { return this.name; }
来源：http://dqn.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://lzx.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://qzg.xuetiantiany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kzf.gotoacloud.top

Ruby: def to_s; @name; end
来源：http://rxj.jinghuilouyu.cn

C#:   public override string ToString() => Name;
来源：http://wkl.bjfxy.top

[G13] 判断对象类型
来源：http://vyq.tarul.cn

Py:   isinstance(u, User)
来源：http://wzo.zhixingplan.top

PHP:  $u instanceof User
来源：http://ioz.sxryk.cn

JS:   u instanceof User
来源：http://apc.ydzc1.top

TS:   u instanceof User
来源：http://swb.birdmap.top

Java: u instanceof User
来源：http://ues.smart0.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://wan.hcnkem.com

Ruby: u.is_a?(User)
来源：http://hsf.xinyue.icu

C#:   u is User
来源：http://xsq.jlsjyb.cn

[G14] 数据类 / record
来源：http://sld.sufxvd.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xfl.ppjwa.cn

PHP:  // 用 readonly 属性模拟
来源：http://shv.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gae.fanxiaobao.xyz

TS:   type User = { name: string; age: number };
来源：http://yfc.yanxiufei.cn

Java: record User(String name, int age) {}
来源：http://pqg.jiagoushi.top

Go:   type User struct { Name string; Age int }
来源：http://ilv.gogol.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lhx.shzxlz.cn

C#:   record User(string Name, int Age);
来源：http://tcv.meibo888.top

[G15] 枚举
来源：http://awr.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dij.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://tnn.chenzaomai.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://frx.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qlx.chenlongwang.top

Java: enum Color { RED, GREEN }
来源：http://vbk.hysaishi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ogg.meibo888.top

Ruby: Color = %i[red green].freeze
来源：http://fkl.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rmn.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://ttg.bjfxy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wui.xylfe.cn

PHP:  get_object_vars($obj);
来源：http://hfg.cucudq.cn

JS:   Object.entries(obj)
来源：http://mwk.epnwcf.com

TS:   Object.entries(obj)
来源：http://ccv.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pkr.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://owg.ctjpmb.com

Ruby: obj.instance_variables
来源：http://fjr.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://vgq.gaohongyu789.top

================================================================================
来源：http://fri.xinyue.icu

H. 异常与错误处理
来源：http://coh.jlsjyb.cn

================================================================================
来源：http://ktu.ppjwa.cn

[H01] try / catch 基础
来源：http://wrr.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yym.gogol.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zmg.shzxlz.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pdu.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pqx.dashuyun.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wyj.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xfk.yvedp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gcl.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lne.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://ait.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://fyx.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rir.daria6918.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wuy.epnwcf.com

TS:   try { f(); } finally { cleanup(); }
来源：http://yfz.shuidangran.top

Java: try { f(); } finally { cleanup(); }
来源：http://lzy.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://awm.gotoacloud.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qlr.jianghu66.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://lzi.xinyue.icu

[H03] 主动抛出异常
来源：http://ubc.redwolf501.top

Py:   raise ValueError("错误信息")
来源：http://qcp.havefunace.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jer.cashguo.top

JS:   throw new Error("错误信息");
来源：http://omh.sxryk.cn

TS:   throw new Error("错误信息");
来源：http://qfc.fktsv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://puw.xziqi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lgp.cqqwz.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://enj.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://rhv.gogol.net.cn

[H04] 自定义异常类型
来源：http://qwp.xziqi.cn

Py:   class MyError(Exception): pass
来源：http://jmu.jqgufenzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://ued.shzxlz.cn

JS:   class MyError extends Error {}
来源：http://ukx.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://oxm.jinghuilouyu.cn

Java: class MyException extends RuntimeException {}
来源：http://vnb.fktsv.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lwy.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://qym.fanxiaobao.xyz

C#:   class MyException : Exception {}
来源：http://ced.sjlbkw.cn

[H05] 捕获特定类型
来源：http://bxy.ydjk.org.cn

Py:   except ValueError as e:
来源：http://okt.nanxinkj.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bww.zycfv.cn

JS:   if (e instanceof TypeError) {}
来源：http://mto.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://lee.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://laj.vqdsnc.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://edm.zhijiandao.cn

Ruby: rescue ArgumentError => e
来源：http://qae.cucudq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tle.guowangkeji.top

[H06] 可选值 / 空值安全访问
来源：http://tfy.daria6918.cn

Py:   value = d.get("k") or default
来源：http://zta.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://mgj.quarkkingdee.top

JS:   obj?.a?.b;  d ?? default
来源：http://ooi.nanxinkj.top

TS:   obj?.a?.b;  d ?? default
来源：http://bob.zycfv.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ndz.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hpu.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://uqt.zhengqikj.top

C#:   obj?.A?.B ?? default
来源：http://dir.fzhhl.top

[H07] 断言
来源：http://hab.andypj.xyz

Py:   assert x > 0, "必须为正"
来源：http://euh.tian-w.cn

PHP:  assert($x > 0);
来源：http://pza.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://tny.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://yfh.hammf.cn

Java: assert x > 0 : "必须为正";
来源：http://xkz.ivvv.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wjk.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://lgk.sweek.top

C#:   Debug.Assert(x > 0);
来源：http://kok.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://zmu.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://wic.daxiang520.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rnd.shangyingyoupin.top

JS:   e.message;  e.stack
来源：http://qer.xziqi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pfg.yongpay.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cup.gzhubu.top

Go:   err.Error()
来源：http://cyn.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://nqx.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://shs.shzxlz.cn

[H09] 带错误码的异常
来源：http://dtx.hammf.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://czb.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ssv.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lwc.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cgo.sweek.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nof.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gpu.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://ouw.chenlongwang.top

C#:   // 自定义异常类中加 Code 属性
来源：http://zss.guowangkeji.top

[H10] 资源自动释放
来源：http://ppd.shuidangran.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ylz.quarkkingdee.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nku.shanyushiyangtech.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lmh.gogol.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nfu.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ofb.yuanzhike.top

Go:   defer f.Close()
来源：http://sdi.gzhubu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sxn.sweek.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://suv.hysaishi.cn

================================================================================
来源：http://arn.nanxuanxn.top

I. 正则表达式
来源：http://dqw.cheryme.top

================================================================================
来源：http://vfn.gaohongyu789.top

[I01] 判断是否匹配
来源：http://pqj.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pjz.chenjidiqi.icu

PHP:  preg_match('/\d+/', $s);
来源：http://ybl.ctjpmb.com

JS:   /\d+/.test(s)
来源：http://etg.gogol.net.cn

TS:   /\d+/.test(s)
来源：http://jwx.cdnleiting.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xif.yj20258.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lmo.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://lyv.shuidangran.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dhl.xziqi.cn

[I02] 提取所有匹配
来源：http://rdr.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://qok.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rzp.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tvg.haohaochexian.top

TS:   s.match(/\d+/g)
来源：http://qms.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rpe.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gam.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://xkf.fzhhl.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hka.shzxlz.cn

[I03] 提取捕获分组
来源：http://xer.yonumen.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vrb.iojbl.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gfq.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://buv.nanxuanxn.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zit.xuanzx.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fih.hfpthk.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wit.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://esb.cheryme.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tzu.cdnleiting.top

[I04] 正则替换
来源：http://wnx.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://xbk.meibo888.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lsl.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://xcf.xziqi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aga.zhijiandao.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hgb.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ehr.hysaishi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tkg.yuanzhike.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gcv.fanxiaobao.xyz

[I05] 按正则拆分
来源：http://vcj.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://meg.haohaochexian.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lxp.wangshuangyany.cn

JS:   s.split(/\s*,\s*/)
来源：http://kyo.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://cqt.sysykeji.top

Java: s.split("\\s*,\\s*")
来源：http://epp.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jnp.jinqigufen.top

Ruby: s.split(/\s*,\s*/)
来源：http://ndp.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vfl.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://siw.mhx1999.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://igr.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yhk.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cye.jqgfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qtu.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vlk.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://llp.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://smd.yj20258.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oyz.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://rdf.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://poz.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dnt.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://btr.nanxuanxn.top

TS:   /error/gim
来源：http://mxe.jiagoushi.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ozu.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eoe.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://epx.yueranfly.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://npx.zhongyouzk.top

[I08] 贪婪与非贪婪匹配
来源：http://fvv.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://axh.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oel.jinghuilouyu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jrl.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mlg.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qxz.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pok.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvi.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qkt.shanyushiyangtech.top

================================================================================
来源：http://jfg.sxryk.cn

J. 日期与时间
来源：http://loy.hcnkem.com

================================================================================
来源：http://zkn.tarul.cn

[J01] 获取当前时间
来源：http://nvu.jyoumei.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bfw.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://otl.jinqigfzy.top

JS:   new Date();  Date.now()
来源：http://zyf.tanke756.top

TS:   new Date();  Date.now()
来源：http://gdy.hammf.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eig.fanxiaobao.xyz

Go:   time.Now()
来源：http://laq.bbcook.cn

Ruby: Time.now
来源：http://rnd.sufxvd.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wwa.316326.xyz

[J02] 格式化输出
来源：http://exo.yj20258.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zpl.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tmk.zhoulong.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rxk.gzhubu.top

TS:   d.toISOString()
来源：http://eln.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jau.zdbjq.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvb.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vxg.ehwqpu.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nvk.jianghu66.top

[J03] 字符串解析为日期
来源：http://bmh.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bgn.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kxd.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://hff.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://fkv.uphjek.com

Java: LocalDate.parse("2024-01-02")
来源：http://cla.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gub.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://kou.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://glf.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://jwo.zycfv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://idz.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cmm.chenzaomai.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fdg.tanke756.top

TS:   Math.floor(Date.now() / 1000)
来源：http://pwy.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://efl.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://eoh.cdnleiting.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lqs.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vtc.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://zxl.chenjidiqi.icu

Py:   now + timedelta(days=7)
来源：http://eqj.yj20258888.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gtq.zycfv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmq.cheryme.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://flb.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://xng.hcnkem.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tig.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://hbk.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://czm.chenjidiqi.icu

[J06] 计算两时间之差
来源：http://pat.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://hoc.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://atd.yanxiufei.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tow.xuanzx.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vwf.pengpengdd.cyou


<!-- 参考信息 -->