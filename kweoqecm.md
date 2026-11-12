代发 wailian999

PHP:  public static function f() {}
来源：http://kmv.ywan-chungtsiang.top

JS:   static f() {}
来源：http://knc.dianchejie.cn

TS:   static f(): void {}
来源：http://pyg.yj20258888.top

Java: static void f() {}
来源：http://wnd.fengsongda.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://jdw.xziqi.cn

Ruby: def self.f; end
来源：http://phd.gzhubu.top

C#:   public static void F() {}
来源：http://kfy.redwolf501.top

[G09] 接口 / 抽象类
来源：http://jrj.xuanzx.com

Py:   from abc import ABC, abstractmethod
来源：http://nsr.yuanzhike.top

PHP:  interface Shape { public function area(): float; }
来源：http://qrk.fktsv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://whs.zdbjq.cn

TS:   interface Shape { area(): number; }
来源：http://vcr.jqgufenzy.top

Java: interface Shape { double area(); }
来源：http://sda.ywan-chungtsiang.top

Go:   type Shape interface { Area() float64 }
来源：http://rjo.tianlin.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qsb.zhengqikj.top

C#:   interface IShape { double Area(); }
来源：http://oep.daria6918.cn

[G10] 访问控制
来源：http://lmc.yangfankeji.com

Py:   约定 _protected / __private（不强制）
来源：http://qiu.jqgufenzy.top

PHP:  public / protected / private
来源：http://vit.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://arb.shuidangran.top

TS:   public / protected / private
来源：http://qfm.hfpthk.cn

Java: public / protected / private / 默认包级
来源：http://pvj.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://crf.hammf.cn

Ruby: public / protected / private
来源：http://aps.kuanghao11.cn

C#:   public / protected / private / internal
来源：http://tlq.fengsongda.top

[G11] getter / setter
来源：http://kyg.fktsv.cn

Py:   @property 与 @x.setter
来源：http://xfj.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://dew.jinghuilouyu.cn

JS:   get name() { return this._name; }
来源：http://ocs.sxryk.cn

TS:   get name(): string { return this._name; }
来源：http://snl.hysaishi.cn

Java: public String getName() { return name; }
来源：http://xsd.ctjpmb.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://tam.mhx1999.top

Ruby: attr_accessor :name
来源：http://nbx.snrcjt.cn

C#:   public string Name { get; set; }
来源：http://gmt.hfpthk.cn

[G12] 对象转字符串
来源：http://tna.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://rec.zhixingplan.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://kwf.pycfn.com

JS:   toString() { return this.name; }
来源：http://wdk.nanxinkj.top

TS:   toString(): string { return this.name; }
来源：http://muj.cucudq.cn

Java: @Override public String toString() { return name; }
来源：http://iwe.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://bjo.wangdashe.top

Ruby: def to_s; @name; end
来源：http://yjm.gzhubu.top

C#:   public override string ToString() => Name;
来源：http://tnv.yonumen.top

[G13] 判断对象类型
来源：http://qeo.9152youxi.cn

Py:   isinstance(u, User)
来源：http://pvm.sysykeji.top

PHP:  $u instanceof User
来源：http://zpt.dashuyun.cn

JS:   u instanceof User
来源：http://doz.birdmap.top

TS:   u instanceof User
来源：http://onn.hammf.cn

Java: u instanceof User
来源：http://fgd.hongshengwenyu.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gvq.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://lad.shanyushiyangkeji.top

C#:   u is User
来源：http://xae.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://ode.gotoacloud.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vua.nanxinkj.top

PHP:  // 用 readonly 属性模拟
来源：http://wae.pengpengdd.cyou

JS:   // 无内置：普通类或对象字面量
来源：http://ajr.pycfn.com

TS:   type User = { name: string; age: number };
来源：http://ccm.kuanghao11.cn

Java: record User(String name, int age) {}
来源：http://jqr.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://mfp.andypj.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jlp.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://who.hammf.cn

[G15] 枚举
来源：http://twf.daria6918.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kkj.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vqu.ppjwa.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hvk.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gyh.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://alg.cucudq.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ofv.dianchejie.cn

Ruby: Color = %i[red green].freeze
来源：http://bin.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wlu.yfazqb.com

[G16] 对象转数组 / 字典
来源：http://hyp.jianghu66.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gcs.yuanzhike.top

PHP:  get_object_vars($obj);
来源：http://xvw.bbcook.cn

JS:   Object.entries(obj)
来源：http://ctr.ehwqpu.com

TS:   Object.entries(obj)
来源：http://ljt.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fir.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ezw.xziqi.cn

Ruby: obj.instance_variables
来源：http://dvj.zhaomingkeji.xyz

C#:   // 用反射或 System.Text.Json
来源：http://ggf.zycfv.cn

================================================================================
来源：http://bwb.wangdashe.top

H. 异常与错误处理
来源：http://bxg.daria6918.cn

================================================================================
来源：http://azm.tian-w.cn

[H01] try / catch 基础
来源：http://sif.sxryk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wos.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mni.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yoc.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rhe.epnwcf.com

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://asy.guowangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rrn.316326.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://udu.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fuy.smart0.xyz

[H02] finally / ensure 收尾
来源：http://eeb.yonumen.top

Py:   try: f()⏎finally: cleanup()
来源：http://gwx.dashuyun.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oxo.gaohongyu789.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yuf.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bbj.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://izl.wangdashe.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://lur.hesvh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bje.hnqzz.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://prg.jqgufenzy.top

[H03] 主动抛出异常
来源：http://xpl.gzhubu.top

Py:   raise ValueError("错误信息")
来源：http://rnl.gotoacloud.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qft.shzxlz.cn

JS:   throw new Error("错误信息");
来源：http://etq.hammf.cn

TS:   throw new Error("错误信息");
来源：http://vbd.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fja.ydjk.org.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ppg.yj202588.top

Ruby: raise ArgumentError, "错误信息"
来源：http://mxt.fzhhl.top

C#:   throw new ArgumentException("错误信息");
来源：http://shb.ivvv.top

[H04] 自定义异常类型
来源：http://gcs.quarkkingdee.top

Py:   class MyError(Exception): pass
来源：http://brm.zhongyouzk.top

PHP:  class MyError extends RuntimeException {}
来源：http://wuu.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://wjb.gotoacloud.top

TS:   class MyError extends Error {}
来源：http://kps.yfazqb.com

Java: class MyException extends RuntimeException {}
来源：http://fas.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://frn.zhaomingkeji.xyz

Ruby: class MyError < StandardError; end
来源：http://pad.shzxlz.cn

C#:   class MyException : Exception {}
来源：http://dio.xuetiantiany.cn

[H05] 捕获特定类型
来源：http://mqi.hesvh.cn

Py:   except ValueError as e:
来源：http://qjb.daria6918.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hep.zhaomingkeji.xyz

JS:   if (e instanceof TypeError) {}
来源：http://dmj.bjfxy.top

TS:   if (e instanceof TypeError) {}
来源：http://kiz.0kj1m.cn

Java: catch (IOException | SQLException e) {}
来源：http://loz.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oir.hammf.cn

Ruby: rescue ArgumentError => e
来源：http://vbr.jianghu66.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://owi.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://xcy.yanxiufei.cn

Py:   value = d.get("k") or default
来源：http://sot.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://uws.chenlongwang.top

JS:   obj?.a?.b;  d ?? default
来源：http://rgw.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://lus.xinyue.icu

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kry.zdqjudy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ctf.nwbrower.top

Ruby: d&.dig(:a, :b)
来源：http://pts.sweek.top

C#:   obj?.A?.B ?? default
来源：http://uki.haohaochexian.top

[H07] 断言
来源：http://ufb.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://voo.yongpay.top

PHP:  assert($x > 0);
来源：http://fxx.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://iie.yj20258888.top

TS:   console.assert(x > 0);
来源：http://gkf.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://zyz.nwbrower.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vkq.52xcode.cn

Ruby: raise "必须为正" unless x > 0
来源：http://koq.ehwqpu.com

C#:   Debug.Assert(x > 0);
来源：http://ogz.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://avn.hongshengwenyu.top

Py:   str(e);  traceback.format_exc()
来源：http://bld.ybcxt.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ber.yj202588.top

JS:   e.message;  e.stack
来源：http://zfx.hywenlv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gvc.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uum.gaohongyu789.top

Go:   err.Error()
来源：http://zdd.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://igr.nanxinkj.top

C#:   e.Message;  e.StackTrace
来源：http://elz.uphjek.com

[H09] 带错误码的异常
来源：http://anp.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gfz.zhixingplan.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://efs.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eoy.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ldl.jlsjyb.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qkn.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iui.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rev.epnwcf.com

C#:   // 自定义异常类中加 Code 属性
来源：http://rus.yangfankeji.com

[H10] 资源自动释放
来源：http://lqs.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jdu.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gfv.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://foi.daxiang520.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nis.yangfankeji.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bck.tian-w.cn

Go:   defer f.Close()
来源：http://woz.snrcjt.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ott.ydzc1.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oes.zhijiandao.cn

================================================================================
来源：http://jee.xingfuxueyuan.xyz

I. 正则表达式
来源：http://kso.haohaochexian.top

================================================================================
来源：http://ckw.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://ctp.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lcc.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://eun.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://oie.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://zvk.0kj1m.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://igz.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://umx.zhaomingkeji.xyz

Ruby: s.match?(/\d+/)
来源：http://mji.gaohongyu789.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gcf.hongshengwenyu.top

[I02] 提取所有匹配
来源：http://kjt.jinqigufen.top

Py:   re.findall(r"\d+", s)
来源：http://cqc.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cnn.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://asw.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://suy.sysykeji.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gzj.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wfm.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://fut.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iis.c1oappe.top

[I03] 提取捕获分组
来源：http://tin.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xpq.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://aon.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cur.ywan-chungtsiang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hkk.vqdsnc.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cwr.dashuyun.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://brs.zhengqikj.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gig.bbcook.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vgu.nanxinkj.top

[I04] 正则替换
来源：http://inb.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gwu.aibaodan.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ikc.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://jku.ctjpmb.com

TS:   s.replace(/\d+/g, "#")
来源：http://foy.daxiang520.top

Java: s.replaceAll("\\d+", "#")
来源：http://lmc.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ija.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tjw.yj20258.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eez.chenzaomai.com

[I05] 按正则拆分
来源：http://mgk.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hph.jinqigufen.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mmr.havefunace.top

JS:   s.split(/\s*,\s*/)
来源：http://vlz.dianchejie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ihc.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://khw.iojbl.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nyu.uphjek.com

Ruby: s.split(/\s*,\s*/)
来源：http://bue.gotoacloud.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sno.shzxlz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oqf.yonumen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mlx.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lqf.xingfuxueyuan.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pla.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ghe.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hcu.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bol.smart0.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://muq.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uvd.yangfankeji.com

[I07] 忽略大小写与多行模式
来源：http://vie.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dpb.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tnp.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gtb.vqdsnc.cn

TS:   /error/gim
来源：http://oan.fktsv.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xbu.tanke756.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fvm.shanyushiyangkeji.top

Ruby: s.scan(/error/i)
来源：http://ejd.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tye.yueranfly.top

[I08] 贪婪与非贪婪匹配
来源：http://waf.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vzy.ydzc1.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lvq.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zlw.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogk.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xfd.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://crz.yanxiufei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yyl.yj202588.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://egf.zhixingplan.top

================================================================================
来源：http://spi.xingfuxueyuan.xyz

J. 日期与时间
来源：http://ybc.aibaodan.cn

================================================================================
来源：http://rtq.vqdsnc.cn

[J01] 获取当前时间
来源：http://zfs.nanxuanxn.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ocw.316326.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yyd.yangfankeji.com

JS:   new Date();  Date.now()
来源：http://juv.aizwys.cn

TS:   new Date();  Date.now()
来源：http://uno.zhongyouzk.top

Java: LocalDateTime.now();  Instant.now()
来源：http://yks.chenjidiqi.icu

Go:   time.Now()
来源：http://meb.zhiwuduotai.top

Ruby: Time.now
来源：http://sbx.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://izz.xziqi.cn

[J02] 格式化输出
来源：http://ozg.nanxuanxn.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jke.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pcf.yj20258.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mwa.cdnleiting.top

TS:   d.toISOString()
来源：http://ruc.xuanzx.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rlu.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ydy.bbcook.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dax.yueranfly.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kqm.hnqzz.top

[J03] 字符串解析为日期
来源：http://kpa.sweek.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cba.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yxu.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://soz.hammf.cn

TS:   new Date("2024-01-02")
来源：http://lme.fktsv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wrq.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ahg.zdbjq.cn

Ruby: Date.parse("2024-01-02")
来源：http://spj.zdbjq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pdt.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://lsv.hywenlv.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wew.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uac.cashguo.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vfu.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vel.chenlongwang.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vqa.jyoumei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nuw.bjfxy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://odi.chenjidiqi.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://grh.cdnleiting.top

[J05] 时间加减（加 7 天）
来源：http://usc.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://ttl.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nbc.zhijiandao.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tzr.wangshuangyany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://snv.jinyuanbaomall.cn

Java: LocalDate.now().plusDays(7)
来源：http://vsw.xinyue.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hzd.nwbrower.top

Ruby: Time.now + 7 * 86400
来源：http://jse.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://mdj.aizwys.cn

[J06] 计算两时间之差
来源：http://ulg.nanxuanxn.top

Py:   (end - start).total_seconds()
来源：http://qnb.sjlbkw.cn

PHP:  $end->diff($start)->days;
来源：http://hxh.yj202588.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mvt.fzhhl.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jdy.shangyingyoupin.top


<!-- 参考信息 -->