代发 wailian999

Ruby: super
来源：http://naw.shanyushiyangtech.top

C#:   base.Greet();
来源：http://wea.shuidangran.top

[G08] 静态方法与属性
来源：http://iah.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wup.hnqzz.top

PHP:  public static function f() {}
来源：http://gmq.hysaishi.cn

JS:   static f() {}
来源：http://pnd.cdnleiting.top

TS:   static f(): void {}
来源：http://jic.c1oappe.top

Java: static void f() {}
来源：http://uqc.meibo888.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bsw.xylfe.cn

Ruby: def self.f; end
来源：http://srh.cqqwz.cn

C#:   public static void F() {}
来源：http://pdv.yongpay.top

[G09] 接口 / 抽象类
来源：http://lem.jinyuanbaomall.cn

Py:   from abc import ABC, abstractmethod
来源：http://ssm.ydjk.org.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mdw.yonumen.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://atd.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://rnw.jiagoushi.top

Java: interface Shape { double area(); }
来源：http://bme.hysaishi.cn

Go:   type Shape interface { Area() float64 }
来源：http://dwx.cqqwz.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hpu.hongshengwenyu.top

C#:   interface IShape { double Area(); }
来源：http://une.yangfankeji.com

[G10] 访问控制
来源：http://qyf.jlsjyb.cn

Py:   约定 _protected / __private（不强制）
来源：http://pqg.tanke756.top

PHP:  public / protected / private
来源：http://nfv.fzhhl.top

JS:   #private 字段；其余公开
来源：http://dqu.fehbvm.com

TS:   public / protected / private
来源：http://sdl.dashuyun.cn

Java: public / protected / private / 默认包级
来源：http://mvt.yongpay.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://edv.tanke756.top

Ruby: public / protected / private
来源：http://eyn.epnwcf.com

C#:   public / protected / private / internal
来源：http://njm.hnqzz.top

[G11] getter / setter
来源：http://rlc.ppjwa.cn

Py:   @property 与 @x.setter
来源：http://yww.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rbw.cheryme.top

JS:   get name() { return this._name; }
来源：http://pyr.sweek.top

TS:   get name(): string { return this._name; }
来源：http://ywt.chenzaomai.com

Java: public String getName() { return name; }
来源：http://vdh.hysaishi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://efb.yfazqb.com

Ruby: attr_accessor :name
来源：http://wex.uphjek.com

C#:   public string Name { get; set; }
来源：http://dxx.pycfn.com

[G12] 对象转字符串
来源：http://lfd.zhoulong.xyz

Py:   def __str__(self): return self.name
来源：http://lnu.gotoacloud.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://uie.xuetiantiany.cn

JS:   toString() { return this.name; }
来源：http://bkn.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://ngg.shuidangran.top

Java: @Override public String toString() { return name; }
来源：http://eve.jyoumei.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qul.316326.xyz

Ruby: def to_s; @name; end
来源：http://wms.bjfxy.top

C#:   public override string ToString() => Name;
来源：http://kym.hfpthk.cn

[G13] 判断对象类型
来源：http://jnp.zhoulong.xyz

Py:   isinstance(u, User)
来源：http://fte.tanke756.top

PHP:  $u instanceof User
来源：http://cct.quarkkingdee.top

JS:   u instanceof User
来源：http://itl.zhongyouzk.top

TS:   u instanceof User
来源：http://axs.sufxvd.cn

Java: u instanceof User
来源：http://lsy.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://eiz.tanke756.top

Ruby: u.is_a?(User)
来源：http://nfw.mhx1999.top

C#:   u is User
来源：http://xkn.sjlbkw.cn

[G14] 数据类 / record
来源：http://crp.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dsq.hywenlv.cn

PHP:  // 用 readonly 属性模拟
来源：http://ect.chenlongwang.top

JS:   // 无内置：普通类或对象字面量
来源：http://zrw.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://hgq.chenzaomai.com

Java: record User(String name, int age) {}
来源：http://ycg.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://hlb.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xhq.tian-w.cn

C#:   record User(string Name, int Age);
来源：http://wic.wangdashe.top

[G15] 枚举
来源：http://zhf.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ifj.ivvv.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pnd.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vty.aibaodan.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cjs.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://yvf.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oks.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://uwu.zhijiandao.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hmm.birdmap.top

[G16] 对象转数组 / 字典
来源：http://vwf.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://kmc.hnqzz.top

PHP:  get_object_vars($obj);
来源：http://jjp.fehbvm.com

JS:   Object.entries(obj)
来源：http://odw.c1oappe.top

TS:   Object.entries(obj)
来源：http://mng.zdqjudy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cog.redwolf501.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qpi.xziqi.cn

Ruby: obj.instance_variables
来源：http://ull.ydzc1.top

C#:   // 用反射或 System.Text.Json
来源：http://oqg.hysaishi.cn

================================================================================
来源：http://adh.jinqigfzy.top

H. 异常与错误处理
来源：http://mcw.vehdjk.com

================================================================================
来源：http://dfw.quarkkingdee.top

[H01] try / catch 基础
来源：http://sqj.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qta.wangshuangyany.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yvm.ehwqpu.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://urx.feifeiyinyue.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aei.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ooo.ehwqpu.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://alx.gotoacloud.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dvo.ydzc1.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jsd.xylfe.cn

[H02] finally / ensure 收尾
来源：http://pjb.yj20258.top

Py:   try: f()⏎finally: cleanup()
来源：http://lww.smart0.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://dbp.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://bbo.hywenlv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gkz.ppjwa.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dvp.ppjwa.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dof.tianlin.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://rnv.ydjk.org.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dys.pengpengdd.cyou

[H03] 主动抛出异常
来源：http://mcy.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://yxj.tianlin.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ccr.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://qkg.ctjpmb.com

TS:   throw new Error("错误信息");
来源：http://pjd.hammf.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hux.fengsongda.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cor.chenzaomai.com

Ruby: raise ArgumentError, "错误信息"
来源：http://kjl.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://hxi.ydjk.org.cn

[H04] 自定义异常类型
来源：http://ckj.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://mjm.dashuyun.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zty.hfpthk.cn

JS:   class MyError extends Error {}
来源：http://wwb.sufxvd.cn

TS:   class MyError extends Error {}
来源：http://end.zhijiandao.cn

Java: class MyException extends RuntimeException {}
来源：http://zue.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fvt.zhongyouzk.top

Ruby: class MyError < StandardError; end
来源：http://zvm.xinyue.icu

C#:   class MyException : Exception {}
来源：http://tdl.quarkkingdee.top

[H05] 捕获特定类型
来源：http://wbk.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://ser.feifeiyinyue.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://him.cdnleiting.top

JS:   if (e instanceof TypeError) {}
来源：http://kiy.ywan-chungtsiang.top

TS:   if (e instanceof TypeError) {}
来源：http://yyy.hongshengwenyu.top

Java: catch (IOException | SQLException e) {}
来源：http://bba.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qku.hywenlv.cn

Ruby: rescue ArgumentError => e
来源：http://hri.redwolf501.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://szj.wangshuangyany.cn

[H06] 可选值 / 空值安全访问
来源：http://slx.hcnkem.com

Py:   value = d.get("k") or default
来源：http://oxc.guowangkeji.top

PHP:  $v = $d["k"] ?? null;
来源：http://ocw.kuanghao11.cn

JS:   obj?.a?.b;  d ?? default
来源：http://str.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zys.hesvh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://smt.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mxn.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://eca.0kj1m.cn

C#:   obj?.A?.B ?? default
来源：http://weq.xuanzx.com

[H07] 断言
来源：http://qsd.dashuyun.cn

Py:   assert x > 0, "必须为正"
来源：http://ksd.hysaishi.cn

PHP:  assert($x > 0);
来源：http://imp.smart0.xyz

JS:   console.assert(x > 0);
来源：http://mak.316326.xyz

TS:   console.assert(x > 0);
来源：http://dzk.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://ocx.yj20258.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vdd.shangyingyoupin.top

Ruby: raise "必须为正" unless x > 0
来源：http://vpj.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://ucm.fehbvm.com

[H08] 获取错误信息与堆栈
来源：http://hyi.bbcook.cn

Py:   str(e);  traceback.format_exc()
来源：http://zhz.havefunace.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nty.ehwqpu.com

JS:   e.message;  e.stack
来源：http://sjt.0kj1m.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bnd.zhixingplan.top

Java: e.getMessage();  e.printStackTrace()
来源：http://mur.jqgufenzy.top

Go:   err.Error()
来源：http://mxr.fanxiaobao.xyz

Ruby: e.message;  e.backtrace
来源：http://fsp.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://gde.0kj1m.cn

[H09] 带错误码的异常
来源：http://pfj.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://psf.tian-w.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mfr.dashuyun.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://por.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mde.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dwm.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rek.zhixingplan.top

Ruby: raise MyError.new("fail", 500)
来源：http://thg.cqqwz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qph.jqgfzy.top

[H10] 资源自动释放
来源：http://byz.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gdh.tian-w.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pdf.jinqigufen.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rna.jqgufenzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eha.cdnleiting.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pkr.yangfankeji.com

Go:   defer f.Close()
来源：http://vov.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zpf.guowangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rlj.jinghuilouyu.cn

================================================================================
来源：http://krb.guowangkeji.top

I. 正则表达式
来源：http://ntw.sweek.top

================================================================================
来源：http://ich.redwolf501.top

[I01] 判断是否匹配
来源：http://blg.wangdashe.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ont.cheryme.top

PHP:  preg_match('/\d+/', $s);
来源：http://oqh.andypj.xyz

JS:   /\d+/.test(s)
来源：http://lkh.yj202588.top

TS:   /\d+/.test(s)
来源：http://wja.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vnu.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ved.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://ent.jianghu66.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hyw.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://mkr.xylfe.cn

Py:   re.findall(r"\d+", s)
来源：http://aoj.nanxinkj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fwu.aibaodan.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tnn.xuetiantiany.cn

TS:   s.match(/\d+/g)
来源：http://ino.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jmr.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xee.tianlin.xyz

Ruby: s.scan(/\d+/)
来源：http://plx.ydjk.org.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zgh.gogol.net.cn

[I03] 提取捕获分组
来源：http://wcz.ybcxt.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://map.epnwcf.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lcg.yuanzhike.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ghq.yj20258888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oll.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hxm.dianchejie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bmp.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iux.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wrg.9152youxi.cn

[I04] 正则替换
来源：http://tol.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wte.hnqzz.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://whv.xuanzx.com

JS:   s.replace(/\d+/g, "#")
来源：http://bae.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://wvi.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://oee.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pyn.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qpa.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://anu.nanxinkj.top

[I05] 按正则拆分
来源：http://lck.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zrk.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vqg.hysaishi.cn

JS:   s.split(/\s*,\s*/)
来源：http://vgu.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://ykx.jqgufenzy.top

Java: s.split("\\s*,\\s*")
来源：http://bwz.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uhv.sufxvd.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jrr.ywan-chungtsiang.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ioc.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tdq.havefunace.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ruf.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qjy.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kyb.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rdz.vqdsnc.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bgk.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hpf.gogol.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jhy.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ofi.shanyushiyangtech.top

[I07] 忽略大小写与多行模式
来源：http://ume.cashguo.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://alu.yongpay.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cfk.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mzy.zhoulong.xyz

TS:   /error/gim
来源：http://wpu.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jre.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aws.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://czw.svipenyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://byl.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://ize.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fmg.yueranfly.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rfv.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mzs.bjfxy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jyz.birdmap.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dud.cucudq.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://szh.cucudq.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dbt.guowangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pyu.aibaodan.cn

================================================================================
来源：http://lnb.cqqwz.cn

J. 日期与时间
来源：http://irr.shuidangran.top

================================================================================
来源：http://eje.xuetiantiany.cn

[J01] 获取当前时间
来源：http://etf.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cob.c1oappe.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rty.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://cok.gotoacloud.top

TS:   new Date();  Date.now()
来源：http://hmm.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://fdz.guannengcc.top

Go:   time.Now()
来源：http://xmg.jinghuilouyu.cn

Ruby: Time.now
来源：http://mgw.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lhd.zhaomingkeji.xyz

[J02] 格式化输出
来源：http://nep.ppjwa.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lat.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://orh.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jbg.sweek.top

TS:   d.toISOString()
来源：http://csv.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mkh.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gbg.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xio.cqqwz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://drd.hnxiangtu.top

[J03] 字符串解析为日期
来源：http://kmn.yvedp.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zus.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mki.sweek.top

JS:   new Date("2024-01-02")
来源：http://egb.ivvv.top

TS:   new Date("2024-01-02")
来源：http://fuy.shangyingyoupin.top

Java: LocalDate.parse("2024-01-02")
来源：http://cil.pengpengdd.cyou

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://znz.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://txp.hywenlv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rai.gaohongyu789.top

[J04] 时间戳与日期互转
来源：http://puy.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qxn.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ikg.iojbl.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mlb.nanxinkj.top

TS:   Math.floor(Date.now() / 1000)
来源：http://max.cucudq.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://dzw.tanke756.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://orq.hnqzz.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jdv.tianlin.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nys.pycfn.com

[J05] 时间加减（加 7 天）
来源：http://jaw.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://ebs.andypj.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://eku.jinyuanbaomall.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yww.ybcxt.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://etq.vehdjk.com

Java: LocalDate.now().plusDays(7)
来源：http://ufi.ydzc1.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://znj.chenlongwang.top

Ruby: Time.now + 7 * 86400
来源：http://ank.mhx1999.top

C#:   DateTime.Now.AddDays(7)
来源：http://isn.hammf.cn

[J06] 计算两时间之差
来源：http://nbo.dashuyun.cn


<!-- 参考信息 -->