代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://rou.smart0.xyz

Ruby: def self.f; end
来源：http://ila.jqgufenzy.top

C#:   public static void F() {}
来源：http://fmh.shangyingyoupin.top

[G09] 接口 / 抽象类
来源：http://seg.316326.xyz

Py:   from abc import ABC, abstractmethod
来源：http://pnz.gotoacloud.top

PHP:  interface Shape { public function area(): float; }
来源：http://lho.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://jim.tarul.cn

TS:   interface Shape { area(): number; }
来源：http://dka.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://ctn.xinyue.icu

Go:   type Shape interface { Area() float64 }
来源：http://pst.xuanzx.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cgx.sweek.top

C#:   interface IShape { double Area(); }
来源：http://xnb.dianchejie.cn

[G10] 访问控制
来源：http://hlg.birdmap.top

Py:   约定 _protected / __private（不强制）
来源：http://xcs.yangfankeji.com

PHP:  public / protected / private
来源：http://iam.shangyingyoupin.top

JS:   #private 字段；其余公开
来源：http://umq.jqgufenzy.top

TS:   public / protected / private
来源：http://oyw.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://wtj.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://kdp.fktsv.cn

Ruby: public / protected / private
来源：http://kpn.yuxming.cn

C#:   public / protected / private / internal
来源：http://fae.ywan-chungtsiang.top

[G11] getter / setter
来源：http://rxa.epnwcf.com

Py:   @property 与 @x.setter
来源：http://jlx.sxryk.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fxa.sxryk.cn

JS:   get name() { return this._name; }
来源：http://fdr.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://ysl.xingfuxueyuan.xyz

Java: public String getName() { return name; }
来源：http://oss.zhixingplan.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ecu.xinyue.icu

Ruby: attr_accessor :name
来源：http://yph.fktsv.cn

C#:   public string Name { get; set; }
来源：http://zfm.jinqigufen.top

[G12] 对象转字符串
来源：http://jyt.dianchejie.cn

Py:   def __str__(self): return self.name
来源：http://gtx.316326.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bwi.pycfn.com

JS:   toString() { return this.name; }
来源：http://dqm.cashguo.top

TS:   toString(): string { return this.name; }
来源：http://fyr.chenjidiqi.icu

Java: @Override public String toString() { return name; }
来源：http://sgs.zhongyouzk.top

Go:   func (u User) String() string { return u.Name }
来源：http://huo.meibo888.top

Ruby: def to_s; @name; end
来源：http://sqm.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://pzy.ehwqpu.com

[G13] 判断对象类型
来源：http://asv.0kj1m.cn

Py:   isinstance(u, User)
来源：http://zgz.yongpay.top

PHP:  $u instanceof User
来源：http://ksh.iojbl.cn

JS:   u instanceof User
来源：http://icw.aibaodan.cn

TS:   u instanceof User
来源：http://rpy.fktsv.cn

Java: u instanceof User
来源：http://tgv.xuetiantiany.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tyw.fktsv.cn

Ruby: u.is_a?(User)
来源：http://zgm.nanxinkj.top

C#:   u is User
来源：http://otf.jlsjyb.cn

[G14] 数据类 / record
来源：http://acs.haohaochexian.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vsb.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://dkb.havefunace.top

JS:   // 无内置：普通类或对象字面量
来源：http://pdj.dashuyun.cn

TS:   type User = { name: string; age: number };
来源：http://asm.daria6918.cn

Java: record User(String name, int age) {}
来源：http://ypu.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://pqo.sysykeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ruf.yangfankeji.com

C#:   record User(string Name, int Age);
来源：http://owq.tianlin.xyz

[G15] 枚举
来源：http://ahk.pengpengdd.cyou

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bbo.mhx1999.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pyq.ctjpmb.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ktm.tanke756.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://apq.sweek.top

Java: enum Color { RED, GREEN }
来源：http://gal.cqqwz.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oyd.cdnleiting.top

Ruby: Color = %i[red green].freeze
来源：http://nkb.jinqigufen.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jfi.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://fhz.hongshengwenyu.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rqi.haohaochexian.top

PHP:  get_object_vars($obj);
来源：http://ows.yfazqb.com

JS:   Object.entries(obj)
来源：http://efl.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://rvt.sysykeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bma.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://etf.ybcxt.top

Ruby: obj.instance_variables
来源：http://gbx.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://mlc.xinyue.icu

================================================================================
来源：http://ukc.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://hwq.fktsv.cn

================================================================================
来源：http://zyn.yangfankeji.com

[H01] try / catch 基础
来源：http://tdg.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ssi.zhengqikj.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ebi.ctjpmb.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cll.dianchejie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vnp.fktsv.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://flh.ivvv.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oho.hongshengwenyu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bxv.cheryme.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pdl.tianlin.xyz

[H02] finally / ensure 收尾
来源：http://suc.shanyushiyangtech.top

Py:   try: f()⏎finally: cleanup()
来源：http://nlh.havefunace.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://nse.dashuyun.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zar.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://aqv.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://hxq.zhixingplan.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sfa.cashguo.top

Ruby: begin; f; ensure; cleanup; end
来源：http://cdn.jyoumei.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gsx.ppjwa.cn

[H03] 主动抛出异常
来源：http://vds.chenjidiqi.icu

Py:   raise ValueError("错误信息")
来源：http://qer.zycfv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qgy.ctjpmb.com

JS:   throw new Error("错误信息");
来源：http://web.gaohongyu789.top

TS:   throw new Error("错误信息");
来源：http://xis.xziqi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://irn.zdbjq.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qtr.sysykeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cmg.fengsongda.top

C#:   throw new ArgumentException("错误信息");
来源：http://fgn.feifeiyinyue.top

[H04] 自定义异常类型
来源：http://ujw.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://vkm.gogol.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pzz.chenjidiqi.icu

JS:   class MyError extends Error {}
来源：http://kzq.ehwqpu.com

TS:   class MyError extends Error {}
来源：http://mnv.guowangkeji.top

Java: class MyException extends RuntimeException {}
来源：http://bbt.feifeiyinyue.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mlk.birdmap.top

Ruby: class MyError < StandardError; end
来源：http://hpw.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://urq.snrcjt.cn

[H05] 捕获特定类型
来源：http://dib.shanyushiyangtech.top

Py:   except ValueError as e:
来源：http://okl.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://znx.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://axu.cashguo.top

TS:   if (e instanceof TypeError) {}
来源：http://fpa.sufxvd.cn

Java: catch (IOException | SQLException e) {}
来源：http://wff.yueranfly.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://snt.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://vgl.jinghuilouyu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://drx.nwbrower.top

[H06] 可选值 / 空值安全访问
来源：http://kug.yuxming.cn

Py:   value = d.get("k") or default
来源：http://fzs.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://yff.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kdy.316326.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://oib.jinqigufen.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://esz.hysaishi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://djp.yueranfly.top

Ruby: d&.dig(:a, :b)
来源：http://uxs.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://dzr.hnxiangtu.top

[H07] 断言
来源：http://gto.pycfn.com

Py:   assert x > 0, "必须为正"
来源：http://oqf.jinqigufen.top

PHP:  assert($x > 0);
来源：http://wde.ctjpmb.com

JS:   console.assert(x > 0);
来源：http://rug.sweek.top

TS:   console.assert(x > 0);
来源：http://oxn.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://alr.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xej.andypj.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://uha.haohaochexian.top

C#:   Debug.Assert(x > 0);
来源：http://wqy.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://eww.mhx1999.top

Py:   str(e);  traceback.format_exc()
来源：http://xvy.9152youxi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jrd.jinghuilouyu.cn

JS:   e.message;  e.stack
来源：http://gct.zhiwuduotai.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://qce.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eym.hywenlv.cn

Go:   err.Error()
来源：http://ugt.hongshengwenyu.top

Ruby: e.message;  e.backtrace
来源：http://cvp.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://lji.bjfxy.top

[H09] 带错误码的异常
来源：http://jmi.meibo888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://izn.zhaomingkeji.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://zjn.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cif.zhixingplan.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qkb.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://byk.aibaodan.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hhh.nwbrower.top

Ruby: raise MyError.new("fail", 500)
来源：http://kgk.316326.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://bdl.bbcook.cn

[H10] 资源自动释放
来源：http://psn.jyoumei.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rxk.yuanzhike.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iks.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bii.gotoacloud.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yds.pengpengdd.cyou

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hym.fengsongda.top

Go:   defer f.Close()
来源：http://lbz.aibaodan.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sms.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pup.yj202588.top

================================================================================
来源：http://rbt.havefunace.top

I. 正则表达式
来源：http://lfb.dashuyun.cn

================================================================================
来源：http://bcw.yangfankeji.com

[I01] 判断是否匹配
来源：http://dad.zhoulong.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gzz.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wlx.zycfv.cn

JS:   /\d+/.test(s)
来源：http://ibm.zycfv.cn

TS:   /\d+/.test(s)
来源：http://awv.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nbn.yongpay.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://eqp.yvedp.cn

Ruby: s.match?(/\d+/)
来源：http://pmh.tarul.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wfz.guannengcc.top

[I02] 提取所有匹配
来源：http://rqx.kuanghao11.cn

Py:   re.findall(r"\d+", s)
来源：http://odh.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xwv.zhongyouzk.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ptf.bbcook.cn

TS:   s.match(/\d+/g)
来源：http://hva.fzhhl.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rat.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sfa.jinqigfzy.top

Ruby: s.scan(/\d+/)
来源：http://vnd.cqqwz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eet.vqdsnc.cn

[I03] 提取捕获分组
来源：http://nfb.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ihw.cheryme.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sqd.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iol.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pmh.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baw.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://svs.xziqi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qzh.vqdsnc.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fwi.svipenyu.cn

[I04] 正则替换
来源：http://cdu.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://wiw.ivvv.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eiz.fktsv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wlp.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hty.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://rrw.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://rcd.kuanghao11.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xaj.daria6918.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vhf.snrcjt.cn

[I05] 按正则拆分
来源：http://ajt.cdnleiting.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vdw.daxiang520.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cty.yonumen.top

JS:   s.split(/\s*,\s*/)
来源：http://itl.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://lus.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://wpw.jiagoushi.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pft.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://kva.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rfe.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nff.pycfn.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tcs.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ela.daria6918.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tzh.aibaodan.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tom.uphjek.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://khe.jinqigufen.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nyp.tarul.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ynn.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mja.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://dcj.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iat.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ysf.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qoc.hywenlv.cn

TS:   /error/gim
来源：http://szv.smart0.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cnl.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jqu.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://mgd.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oop.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://qqf.jinqigfzy.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hud.xylfe.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xxm.pycfn.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://apq.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hmq.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://utw.ydzc1.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zjm.dashuyun.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jmc.9152youxi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uap.aizwys.cn

================================================================================
来源：http://wyx.ivvv.top

J. 日期与时间
来源：http://ltt.yvedp.cn

================================================================================
来源：http://gey.cdnleiting.top

[J01] 获取当前时间
来源：http://ojc.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://obd.hywenlv.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wci.jinqigufen.top

JS:   new Date();  Date.now()
来源：http://sdb.pengpengdd.cyou

TS:   new Date();  Date.now()
来源：http://tif.ppjwa.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://paf.hammf.cn

Go:   time.Now()
来源：http://hti.9152youxi.cn

Ruby: Time.now
来源：http://foe.birdmap.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://stq.wangshuangyany.cn

[J02] 格式化输出
来源：http://zbe.fengsongda.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cqq.tianlin.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qpa.dashuyun.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oba.hesvh.cn

TS:   d.toISOString()
来源：http://ori.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wpx.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sap.ydjk.org.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://alv.bbcook.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jjh.xuanzx.com

[J03] 字符串解析为日期
来源：http://qhw.mhx1999.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fut.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nww.yanxiufei.cn

JS:   new Date("2024-01-02")
来源：http://kqs.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://ged.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://nkh.zdbjq.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jfk.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://nau.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rzp.smart0.xyz

[J04] 时间戳与日期互转
来源：http://rvb.nanxuanxn.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vgj.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://uth.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nsg.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ddd.dianchejie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ear.andypj.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ttw.yfazqb.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sdg.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ldp.fktsv.cn

[J05] 时间加减（加 7 天）
来源：http://xrj.zhongyouzk.top

Py:   now + timedelta(days=7)
来源：http://pnz.ywan-chungtsiang.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://slq.pengpengdd.cyou

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xyo.redwolf501.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pyg.vqdsnc.cn

Java: LocalDate.now().plusDays(7)
来源：http://mtj.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xsn.wangshuangyany.cn

Ruby: Time.now + 7 * 86400
来源：http://yyd.zdqjudy.top

C#:   DateTime.Now.AddDays(7)
来源：http://cuc.cdnleiting.top

[J06] 计算两时间之差
来源：http://aoy.316326.xyz

Py:   (end - start).total_seconds()
来源：http://krd.ydjk.org.cn

PHP:  $end->diff($start)->days;
来源：http://fmr.andypj.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://asv.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mks.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://ydz.jinghuilouyu.cn

Go:   end.Sub(start).Hours()
来源：http://tss.yvedp.cn

Ruby: end - start                 # 返回秒数
来源：http://dbk.shangyingyoupin.top

C#:   (end - start).TotalSeconds
来源：http://yii.pengpengdd.cyou


<!-- 参考信息 -->