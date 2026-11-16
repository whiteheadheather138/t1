代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://qez.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://dgk.sxryk.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ypd.yongpay.top

TS:   interface Shape { area(): number; }
来源：http://cfn.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://cak.shanyushiyangkeji.top

Go:   type Shape interface { Area() float64 }
来源：http://sjg.haohaochexian.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://flm.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://gwm.cheryme.top

[G10] 访问控制
来源：http://gss.hywenlv.cn

Py:   约定 _protected / __private（不强制）
来源：http://vru.ybcxt.top

PHP:  public / protected / private
来源：http://bqj.jinyuanbaomall.cn

JS:   #private 字段；其余公开
来源：http://jpc.aibaodan.cn

TS:   public / protected / private
来源：http://jct.xziqi.cn

Java: public / protected / private / 默认包级
来源：http://rjo.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pig.mhx1999.top

Ruby: public / protected / private
来源：http://vbv.sysykeji.top

C#:   public / protected / private / internal
来源：http://ria.nwbrower.top

[G11] getter / setter
来源：http://wry.0kj1m.cn

Py:   @property 与 @x.setter
来源：http://baj.aizwys.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://quz.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://woj.hfpthk.cn

TS:   get name(): string { return this._name; }
来源：http://gfa.0kj1m.cn

Java: public String getName() { return name; }
来源：http://fhu.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://euk.jlsjyb.cn

Ruby: attr_accessor :name
来源：http://qkl.aibaodan.cn

C#:   public string Name { get; set; }
来源：http://enz.chenzaomai.com

[G12] 对象转字符串
来源：http://jet.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://zza.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hrs.xuanzx.com

JS:   toString() { return this.name; }
来源：http://zze.jinqigfzy.top

TS:   toString(): string { return this.name; }
来源：http://rhx.yuxming.cn

Java: @Override public String toString() { return name; }
来源：http://ffa.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://wkt.hesvh.cn

Ruby: def to_s; @name; end
来源：http://cgz.vehdjk.com

C#:   public override string ToString() => Name;
来源：http://bsg.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://lib.dianchejie.cn

Py:   isinstance(u, User)
来源：http://cje.aibaodan.cn

PHP:  $u instanceof User
来源：http://cxl.aibaodan.cn

JS:   u instanceof User
来源：http://njs.hcnkem.com

TS:   u instanceof User
来源：http://uvu.gzhubu.top

Java: u instanceof User
来源：http://xsd.ybcxt.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xtx.bjfxy.top

Ruby: u.is_a?(User)
来源：http://afm.yonumen.top

C#:   u is User
来源：http://zma.xuanzx.com

[G14] 数据类 / record
来源：http://epx.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jpv.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://zbq.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://hkp.yuanzhike.top

TS:   type User = { name: string; age: number };
来源：http://hdd.yj202588.top

Java: record User(String name, int age) {}
来源：http://coq.zhoulong.xyz

Go:   type User struct { Name string; Age int }
来源：http://mzj.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://usu.jinqigfzy.top

C#:   record User(string Name, int Age);
来源：http://ldx.pengpengdd.cyou

[G15] 枚举
来源：http://pvi.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hyw.shzxlz.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://umc.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pwc.svipenyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nvy.hnxiangtu.top

Java: enum Color { RED, GREEN }
来源：http://pdn.shanyushiyangkeji.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gmn.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://uxq.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://suv.ybcxt.top

[G16] 对象转数组 / 字典
来源：http://wpx.jinyuanbaomall.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nzo.yj202588.top

PHP:  get_object_vars($obj);
来源：http://uxe.zdqjudy.top

JS:   Object.entries(obj)
来源：http://wqb.ctjpmb.com

TS:   Object.entries(obj)
来源：http://yod.sxryk.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://obt.gzhubu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zmk.mhx1999.top

Ruby: obj.instance_variables
来源：http://whm.52xcode.cn

C#:   // 用反射或 System.Text.Json
来源：http://zrh.fzhhl.top

================================================================================
来源：http://dys.jianghu66.top

H. 异常与错误处理
来源：http://cqw.tian-w.cn

================================================================================
来源：http://ywf.sjlbkw.cn

[H01] try / catch 基础
来源：http://okf.quarkkingdee.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tqu.yj20258888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qwh.feifeiyinyue.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://env.hnxiangtu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://irt.zhongyouzk.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qwt.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wtp.hammf.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ibn.cdnleiting.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hpb.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://lez.cqqwz.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mmb.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://mpz.hammf.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ddi.chenlongwang.top

TS:   try { f(); } finally { cleanup(); }
来源：http://eeg.fengsongda.top

Java: try { f(); } finally { cleanup(); }
来源：http://hhk.xinyue.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://jfz.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://epy.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://mhh.gotoacloud.top

[H03] 主动抛出异常
来源：http://mvf.yj202588.top

Py:   raise ValueError("错误信息")
来源：http://crp.ivvv.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://txl.yanxiufei.cn

JS:   throw new Error("错误信息");
来源：http://vgr.chenlongwang.top

TS:   throw new Error("错误信息");
来源：http://dnu.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mdt.shuidangran.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vqt.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://abw.chenzaomai.com

C#:   throw new ArgumentException("错误信息");
来源：http://yeq.kuanghao11.cn

[H04] 自定义异常类型
来源：http://eyb.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://eiy.hongshengwenyu.top

PHP:  class MyError extends RuntimeException {}
来源：http://xub.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://zpf.hongshengwenyu.top

TS:   class MyError extends Error {}
来源：http://zac.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://jic.ywan-chungtsiang.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lxr.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://zom.zhengqikj.top

C#:   class MyException : Exception {}
来源：http://iwi.ppjwa.cn

[H05] 捕获特定类型
来源：http://dad.ywan-chungtsiang.top

Py:   except ValueError as e:
来源：http://pwd.hongshengwenyu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oin.yfazqb.com

JS:   if (e instanceof TypeError) {}
来源：http://zol.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://yad.hcnkem.com

Java: catch (IOException | SQLException e) {}
来源：http://xpo.c1oappe.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://age.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://udq.hnqzz.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hpx.ppjwa.cn

[H06] 可选值 / 空值安全访问
来源：http://qnb.gogol.net.cn

Py:   value = d.get("k") or default
来源：http://shl.aizwys.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xjp.cheryme.top

JS:   obj?.a?.b;  d ?? default
来源：http://nct.pycfn.com

TS:   obj?.a?.b;  d ?? default
来源：http://htj.yvedp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lcz.shzxlz.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rxh.zhoulong.xyz

Ruby: d&.dig(:a, :b)
来源：http://bzf.hywenlv.cn

C#:   obj?.A?.B ?? default
来源：http://hja.hfpthk.cn

[H07] 断言
来源：http://ang.ehwqpu.com

Py:   assert x > 0, "必须为正"
来源：http://lsm.c1oappe.top

PHP:  assert($x > 0);
来源：http://joj.jqgufenzy.top

JS:   console.assert(x > 0);
来源：http://jvg.wangdashe.top

TS:   console.assert(x > 0);
来源：http://clu.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://iaz.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lgf.epnwcf.com

Ruby: raise "必须为正" unless x > 0
来源：http://oqz.cucudq.cn

C#:   Debug.Assert(x > 0);
来源：http://dol.xinyue.icu

[H08] 获取错误信息与堆栈
来源：http://wkl.nwbrower.top

Py:   str(e);  traceback.format_exc()
来源：http://zpf.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ivs.haohaochexian.top

JS:   e.message;  e.stack
来源：http://txq.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://nwo.zhoulong.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://jwe.hywenlv.cn

Go:   err.Error()
来源：http://ooh.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://xuh.shzxlz.cn

C#:   e.Message;  e.StackTrace
来源：http://ngv.ybcxt.top

[H09] 带错误码的异常
来源：http://uun.aizwys.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://inv.shangyingyoupin.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://dlm.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mnu.c1oappe.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ily.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ntw.ctjpmb.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kwm.zdqjudy.top

Ruby: raise MyError.new("fail", 500)
来源：http://lrs.nwbrower.top

C#:   // 自定义异常类中加 Code 属性
来源：http://jgr.aizwys.cn

[H10] 资源自动释放
来源：http://tgp.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xeo.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wpe.jyoumei.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jyb.zhengqikj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wun.ybcxt.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mde.c1oappe.top

Go:   defer f.Close()
来源：http://hyk.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://npv.ydjk.org.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jqc.sysykeji.top

================================================================================
来源：http://qsi.wangdashe.top

I. 正则表达式
来源：http://bxr.jlsjyb.cn

================================================================================
来源：http://bwa.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://qmu.cqqwz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ixh.yueranfly.top

PHP:  preg_match('/\d+/', $s);
来源：http://oqx.xylfe.cn

JS:   /\d+/.test(s)
来源：http://nyv.jqgfzy.top

TS:   /\d+/.test(s)
来源：http://qpo.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nwb.jqgfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xxi.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://qhk.52xcode.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cff.shuidangran.top

[I02] 提取所有匹配
来源：http://biu.birdmap.top

Py:   re.findall(r"\d+", s)
来源：http://lup.zhongyouzk.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cmb.xinyue.icu

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qza.cdnleiting.top

TS:   s.match(/\d+/g)
来源：http://xig.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ubm.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cmj.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://tzt.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eao.wangshuangyany.cn

[I03] 提取捕获分组
来源：http://mrr.haohaochexian.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lfo.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sdn.vehdjk.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://afa.guannengcc.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vra.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xpm.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ohr.hnqzz.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qij.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mlf.yj202588.top

[I04] 正则替换
来源：http://loc.jqgfzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wsy.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mru.meibo888.top

JS:   s.replace(/\d+/g, "#")
来源：http://qqd.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://aub.sjlbkw.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kgi.andypj.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://rpj.52xcode.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qhd.hnxiangtu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gjw.52xcode.cn

[I05] 按正则拆分
来源：http://vom.shuidangran.top

Py:   re.split(r"\s*,\s*", s)
来源：http://syq.guowangkeji.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://iby.yueranfly.top

JS:   s.split(/\s*,\s*/)
来源：http://jjr.0kj1m.cn

TS:   s.split(/\s*,\s*/)
来源：http://hlr.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://lbm.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nle.feifeiyinyue.top

Ruby: s.split(/\s*,\s*/)
来源：http://eum.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://myq.vehdjk.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ptg.xylfe.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://izg.cheryme.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tnw.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lzo.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ejz.ehwqpu.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wzl.chenlongwang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ksb.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yyb.zhaomingkeji.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dgs.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://sos.haohaochexian.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fkj.yueranfly.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ecq.ehwqpu.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nzj.yvedp.cn

TS:   /error/gim
来源：http://jhl.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gjo.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kwq.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://giz.gotoacloud.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hdw.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://skp.zdqjudy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cgi.0kj1m.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mtq.ctjpmb.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wkh.sysykeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://guw.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://upp.jqgfzy.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://skx.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wqn.dianchejie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ptc.sufxvd.cn

================================================================================
来源：http://ead.zhiwuduotai.top

J. 日期与时间
来源：http://hdg.shanyushiyangkeji.top

================================================================================
来源：http://rgv.sxryk.cn

[J01] 获取当前时间
来源：http://jch.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hsq.yvedp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nas.yonumen.top

JS:   new Date();  Date.now()
来源：http://ain.haohaochexian.top

TS:   new Date();  Date.now()
来源：http://rmi.jinyuanbaomall.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sib.sxryk.cn

Go:   time.Now()
来源：http://rgf.havefunace.top

Ruby: Time.now
来源：http://kee.pycfn.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qtx.guannengcc.top

[J02] 格式化输出
来源：http://cyb.redwolf501.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pnn.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://scw.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lyz.tianlin.xyz

TS:   d.toISOString()
来源：http://tkz.chenjidiqi.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mhc.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vxc.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dgt.guannengcc.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nva.zycfv.cn

[J03] 字符串解析为日期
来源：http://zlx.pycfn.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://oax.svipenyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://his.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://rkn.smart0.xyz

TS:   new Date("2024-01-02")
来源：http://hdc.9152youxi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jeo.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vqw.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://lzg.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ile.cqqwz.cn

[J04] 时间戳与日期互转
来源：http://dsy.shanyushiyangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ejq.shzxlz.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kgs.yvedp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dly.fktsv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://iev.zhongyouzk.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tkg.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vok.redwolf501.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://icg.uphjek.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jjv.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://nmi.yonumen.top

Py:   now + timedelta(days=7)
来源：http://vxr.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://gfh.svipenyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ifp.meibo888.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mgf.hfpthk.cn

Java: LocalDate.now().plusDays(7)
来源：http://hcd.vqdsnc.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vay.ppjwa.cn

Ruby: Time.now + 7 * 86400
来源：http://pxt.cheryme.top

C#:   DateTime.Now.AddDays(7)
来源：http://rub.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://ghj.fehbvm.com

Py:   (end - start).total_seconds()
来源：http://tcp.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://aas.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jjj.zhiwuduotai.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zyl.sxryk.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pmu.yj20258.top

Go:   end.Sub(start).Hours()
来源：http://hmz.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://ecs.daxiang520.top

C#:   (end - start).TotalSeconds
来源：http://yns.nwbrower.top

[J07] 比较两个日期
来源：http://jjt.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://diu.xziqi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qta.zycfv.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zbo.daria6918.cn


<!-- 参考信息 -->