代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://btj.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gyp.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uxl.ppjwa.cn

TS:   interface Shape { area(): number; }
来源：http://sdu.c1oappe.top

Java: interface Shape { double area(); }
来源：http://mna.tianlin.xyz

Go:   type Shape interface { Area() float64 }
来源：http://cck.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://grh.nanxuanxn.top

C#:   interface IShape { double Area(); }
来源：http://wga.zdqjudy.top

[G10] 访问控制
来源：http://udf.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://mnd.nanxuanxn.top

PHP:  public / protected / private
来源：http://lcv.fktsv.cn

JS:   #private 字段；其余公开
来源：http://fec.zhijiandao.cn

TS:   public / protected / private
来源：http://xfv.jianghu66.top

Java: public / protected / private / 默认包级
来源：http://sen.zhongyouzk.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://yfc.xuetiantiany.cn

Ruby: public / protected / private
来源：http://hro.yonumen.top

C#:   public / protected / private / internal
来源：http://lqt.wangdashe.top

[G11] getter / setter
来源：http://nbf.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://ozl.jyoumei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wxg.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://ljw.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://ukh.yonumen.top

Java: public String getName() { return name; }
来源：http://vpa.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ili.zdqjudy.top

Ruby: attr_accessor :name
来源：http://ljg.quarkkingdee.top

C#:   public string Name { get; set; }
来源：http://qmy.xylfe.cn

[G12] 对象转字符串
来源：http://rfi.ydjk.org.cn

Py:   def __str__(self): return self.name
来源：http://kuq.fzhhl.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://jny.zhongyouzk.top

JS:   toString() { return this.name; }
来源：http://dqs.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://utw.snrcjt.cn

Java: @Override public String toString() { return name; }
来源：http://vkv.aibaodan.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aso.yj20258.top

Ruby: def to_s; @name; end
来源：http://iha.zycfv.cn

C#:   public override string ToString() => Name;
来源：http://ghs.yueranfly.top

[G13] 判断对象类型
来源：http://mma.jinyuanbaomall.cn

Py:   isinstance(u, User)
来源：http://wyi.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://lee.aizwys.cn

JS:   u instanceof User
来源：http://axq.jlsjyb.cn

TS:   u instanceof User
来源：http://ymc.chenlongwang.top

Java: u instanceof User
来源：http://vqd.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nlh.uphjek.com

Ruby: u.is_a?(User)
来源：http://ryh.gzhubu.top

C#:   u is User
来源：http://rus.gogol.net.cn

[G14] 数据类 / record
来源：http://kky.jianghu66.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gly.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://vwt.guannengcc.top

JS:   // 无内置：普通类或对象字面量
来源：http://nnj.sufxvd.cn

TS:   type User = { name: string; age: number };
来源：http://fhq.jqgufenzy.top

Java: record User(String name, int age) {}
来源：http://gbk.nanxuanxn.top

Go:   type User struct { Name string; Age int }
来源：http://kwf.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gnl.sysykeji.top

C#:   record User(string Name, int Age);
来源：http://hpb.vehdjk.com

[G15] 枚举
来源：http://juj.shzxlz.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xee.bjfxy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wfi.zycfv.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vid.jiagoushi.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://joc.cashguo.top

Java: enum Color { RED, GREEN }
来源：http://rxr.wangshuangyany.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zbm.smart0.xyz

Ruby: Color = %i[red green].freeze
来源：http://iuv.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dhu.hnxiangtu.top

[G16] 对象转数组 / 字典
来源：http://ddj.guowangkeji.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://shl.yuxming.cn

PHP:  get_object_vars($obj);
来源：http://zpm.jqgufenzy.top

JS:   Object.entries(obj)
来源：http://mhs.sufxvd.cn

TS:   Object.entries(obj)
来源：http://xuf.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tek.xinyue.icu

Go:   // 手写转换，或用 mapstructure 库
来源：http://mew.hammf.cn

Ruby: obj.instance_variables
来源：http://xbs.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://pia.zhiwuduotai.top

================================================================================
来源：http://nnv.andypj.xyz

H. 异常与错误处理
来源：http://nnn.jinqigufen.top

================================================================================
来源：http://srd.vqdsnc.cn

[H01] try / catch 基础
来源：http://rgq.chenzaomai.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ytl.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hym.vqdsnc.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ylh.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tib.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bdb.smart0.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ljc.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wgy.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tcd.chenzaomai.com

[H02] finally / ensure 收尾
来源：http://eot.hammf.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uqf.zycfv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://meq.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kug.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rzq.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://mgx.9152youxi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://abr.hammf.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zsc.havefunace.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ibh.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://wzz.jinqigufen.top

Py:   raise ValueError("错误信息")
来源：http://udo.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rpz.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://jgq.mhx1999.top

TS:   throw new Error("错误信息");
来源：http://utt.fzhhl.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://lku.daria6918.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ktj.chenjidiqi.icu

Ruby: raise ArgumentError, "错误信息"
来源：http://jmt.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://obf.tanke756.top

[H04] 自定义异常类型
来源：http://vqw.ppjwa.cn

Py:   class MyError(Exception): pass
来源：http://idp.ybcxt.top

PHP:  class MyError extends RuntimeException {}
来源：http://qmv.c1oappe.top

JS:   class MyError extends Error {}
来源：http://lxc.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://hyx.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://poa.zdqjudy.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vzj.xylfe.cn

Ruby: class MyError < StandardError; end
来源：http://atj.chenzaomai.com

C#:   class MyException : Exception {}
来源：http://sqf.jqgufenzy.top

[H05] 捕获特定类型
来源：http://xdu.guowangkeji.top

Py:   except ValueError as e:
来源：http://ghv.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pjp.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://cno.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://fft.ydjk.org.cn

Java: catch (IOException | SQLException e) {}
来源：http://rko.hcnkem.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ogy.jqgfzy.top

Ruby: rescue ArgumentError => e
来源：http://epf.ctjpmb.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mhp.zhijiandao.cn

[H06] 可选值 / 空值安全访问
来源：http://fiq.cqqwz.cn

Py:   value = d.get("k") or default
来源：http://lrl.hongshengwenyu.top

PHP:  $v = $d["k"] ?? null;
来源：http://qqk.hysaishi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mni.epnwcf.com

TS:   obj?.a?.b;  d ?? default
来源：http://osa.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xly.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gco.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://vtb.sufxvd.cn

C#:   obj?.A?.B ?? default
来源：http://jlq.hysaishi.cn

[H07] 断言
来源：http://zpn.shzxlz.cn

Py:   assert x > 0, "必须为正"
来源：http://mfn.aibaodan.cn

PHP:  assert($x > 0);
来源：http://oxd.tanke756.top

JS:   console.assert(x > 0);
来源：http://uha.jinghuilouyu.cn

TS:   console.assert(x > 0);
来源：http://gcm.hysaishi.cn

Java: assert x > 0 : "必须为正";
来源：http://gsk.yj20258888.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://aeo.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://crt.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://bce.yj202588.top

[H08] 获取错误信息与堆栈
来源：http://ynu.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://suo.hysaishi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bwl.birdmap.top

JS:   e.message;  e.stack
来源：http://uvv.gzhubu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cpn.tanke756.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xym.meibo888.top

Go:   err.Error()
来源：http://adl.sweek.top

Ruby: e.message;  e.backtrace
来源：http://gum.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://vau.yfazqb.com

[H09] 带错误码的异常
来源：http://nzw.c1oappe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lnk.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://rio.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://iic.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ckf.sysykeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ztl.gaohongyu789.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://umc.hcnkem.com

Ruby: raise MyError.new("fail", 500)
来源：http://ias.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tas.sweek.top

[H10] 资源自动释放
来源：http://mvs.shanyushiyangkeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://dkv.shangyingyoupin.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yfv.wangshuangyany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xyp.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uoc.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zpy.zhijiandao.cn

Go:   defer f.Close()
来源：http://ihs.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rqj.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vdg.andypj.xyz

================================================================================
来源：http://xwy.zhaomingkeji.xyz

I. 正则表达式
来源：http://pik.hywenlv.cn

================================================================================
来源：http://ucb.hcnkem.com

[I01] 判断是否匹配
来源：http://ejq.ivvv.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ujl.yuanzhike.top

PHP:  preg_match('/\d+/', $s);
来源：http://ejr.gaohongyu789.top

JS:   /\d+/.test(s)
来源：http://pen.chenzaomai.com

TS:   /\d+/.test(s)
来源：http://ybi.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rtk.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ilf.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://zdt.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gdp.yj202588.top

[I02] 提取所有匹配
来源：http://lnz.uphjek.com

Py:   re.findall(r"\d+", s)
来源：http://vaw.cashguo.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://urc.aizwys.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xlx.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://bzx.zhoulong.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xua.uphjek.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nfh.9152youxi.cn

Ruby: s.scan(/\d+/)
来源：http://wvn.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qbn.c1oappe.top

[I03] 提取捕获分组
来源：http://vjg.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ovw.xuanzx.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vyr.zhengqikj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://emy.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ooo.ydjk.org.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tkt.ybcxt.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qmp.hysaishi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pdp.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fom.nanxinkj.top

[I04] 正则替换
来源：http://emq.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uyp.epnwcf.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://slw.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jkx.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://ept.gzhubu.top

Java: s.replaceAll("\\d+", "#")
来源：http://kcr.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://cpn.zhengqikj.top

Ruby: s.gsub(/\d+/, "#")
来源：http://iew.52xcode.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://val.zdbjq.cn

[I05] 按正则拆分
来源：http://owy.havefunace.top

Py:   re.split(r"\s*,\s*", s)
来源：http://frr.cheryme.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xng.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://ikt.tarul.cn

TS:   s.split(/\s*,\s*/)
来源：http://bcr.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://tuu.fktsv.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kfw.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://pao.0kj1m.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blp.redwolf501.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://psz.dashuyun.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rai.smart0.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gts.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oeg.fktsv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dkq.zhengqikj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kpx.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kxt.yongpay.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kco.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nsu.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://tgh.fktsv.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wdz.guannengcc.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mzx.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vce.shanyushiyangtech.top

TS:   /error/gim
来源：http://zks.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ggx.sweek.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bgl.havefunace.top

Ruby: s.scan(/error/i)
来源：http://mem.52xcode.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://doh.fanxiaobao.xyz

[I08] 贪婪与非贪婪匹配
来源：http://dsq.ybcxt.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rsq.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://npn.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://avh.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wqc.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://smp.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rps.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://syk.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vgs.ydjk.org.cn

================================================================================
来源：http://jbk.xylfe.cn

J. 日期与时间
来源：http://abl.yvedp.cn

================================================================================
来源：http://lij.0kj1m.cn

[J01] 获取当前时间
来源：http://bgm.316326.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://ekx.dianchejie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fth.yuxming.cn

JS:   new Date();  Date.now()
来源：http://krq.iojbl.cn

TS:   new Date();  Date.now()
来源：http://rzq.sysykeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bsd.pycfn.com

Go:   time.Now()
来源：http://dec.shuidangran.top

Ruby: Time.now
来源：http://yem.ivvv.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gst.cdnleiting.top

[J02] 格式化输出
来源：http://evu.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lda.vehdjk.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uag.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gkv.jinqigfzy.top

TS:   d.toISOString()
来源：http://myy.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bso.hesvh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wzl.c1oappe.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ixk.vqdsnc.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pwc.wangdashe.top

[J03] 字符串解析为日期
来源：http://hac.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yzk.aibaodan.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pvm.jinqigufen.top

JS:   new Date("2024-01-02")
来源：http://xwq.yongpay.top

TS:   new Date("2024-01-02")
来源：http://jqa.sufxvd.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dky.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wsk.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://rae.zhixingplan.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://glw.hfpthk.cn

[J04] 时间戳与日期互转
来源：http://rkm.pycfn.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ukz.yangfankeji.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nvi.hesvh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yrn.hongshengwenyu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zsi.yuanzhike.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://noh.cdnleiting.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rye.gotoacloud.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qpt.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qcw.zhaomingkeji.xyz

[J05] 时间加减（加 7 天）
来源：http://czy.sufxvd.cn

Py:   now + timedelta(days=7)
来源：http://hek.zhongyouzk.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ppl.haohaochexian.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://uzx.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dii.shzxlz.cn

Java: LocalDate.now().plusDays(7)
来源：http://jqh.yj202588.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vtx.316326.xyz

Ruby: Time.now + 7 * 86400
来源：http://akz.zhijiandao.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yph.ivvv.top

[J06] 计算两时间之差
来源：http://lam.yongpay.top

Py:   (end - start).total_seconds()
来源：http://aqx.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://dbi.shanyushiyangtech.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fnl.jlsjyb.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ink.yuxming.cn

Java: Duration.between(start, end).toSeconds()
来源：http://uxr.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://imm.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://waa.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://wjw.c1oappe.top

[J07] 比较两个日期
来源：http://lrk.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://hhh.shanyushiyangkeji.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ubb.daria6918.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wnv.ybcxt.top


<!-- 参考信息 -->