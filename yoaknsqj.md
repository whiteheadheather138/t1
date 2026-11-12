代发 wailian999

Java: interface Shape { double area(); }
来源：http://adg.vqdsnc.cn

Go:   type Shape interface { Area() float64 }
来源：http://scv.fengsongda.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rvi.pycfn.com

C#:   interface IShape { double Area(); }
来源：http://ndx.mhx1999.top

[G10] 访问控制
来源：http://uns.zhoulong.xyz

Py:   约定 _protected / __private（不强制）
来源：http://evu.ywan-chungtsiang.top

PHP:  public / protected / private
来源：http://qgj.mhx1999.top

JS:   #private 字段；其余公开
来源：http://lja.jianghu66.top

TS:   public / protected / private
来源：http://fpg.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://ytl.haohaochexian.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://ksw.c1oappe.top

Ruby: public / protected / private
来源：http://vqv.jqgufenzy.top

C#:   public / protected / private / internal
来源：http://ycw.iojbl.cn

[G11] getter / setter
来源：http://upi.sjlbkw.cn

Py:   @property 与 @x.setter
来源：http://biq.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://drv.xuanzx.com

JS:   get name() { return this._name; }
来源：http://rmv.svipenyu.cn

TS:   get name(): string { return this._name; }
来源：http://qtr.sufxvd.cn

Java: public String getName() { return name; }
来源：http://qkj.yangfankeji.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://lci.meibo888.top

Ruby: attr_accessor :name
来源：http://pvh.pycfn.com

C#:   public string Name { get; set; }
来源：http://eyv.zhoulong.xyz

[G12] 对象转字符串
来源：http://kkl.shuidangran.top

Py:   def __str__(self): return self.name
来源：http://wya.daria6918.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hmd.fanxiaobao.xyz

JS:   toString() { return this.name; }
来源：http://llm.sufxvd.cn

TS:   toString(): string { return this.name; }
来源：http://pkq.xylfe.cn

Java: @Override public String toString() { return name; }
来源：http://ehq.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://aqx.shanyushiyangtech.top

Ruby: def to_s; @name; end
来源：http://hpe.yj20258.top

C#:   public override string ToString() => Name;
来源：http://sfv.sxryk.cn

[G13] 判断对象类型
来源：http://sbf.yuxming.cn

Py:   isinstance(u, User)
来源：http://iuf.zdbjq.cn

PHP:  $u instanceof User
来源：http://guy.sysykeji.top

JS:   u instanceof User
来源：http://rad.ydzc1.top

TS:   u instanceof User
来源：http://tlf.yangfankeji.com

Java: u instanceof User
来源：http://ybk.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://zwb.shanyushiyangtech.top

Ruby: u.is_a?(User)
来源：http://rja.hfpthk.cn

C#:   u is User
来源：http://mfw.zdqjudy.top

[G14] 数据类 / record
来源：http://izs.nanxinkj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fkh.yonumen.top

PHP:  // 用 readonly 属性模拟
来源：http://xnz.hysaishi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zav.chenlongwang.top

TS:   type User = { name: string; age: number };
来源：http://ioc.pycfn.com

Java: record User(String name, int age) {}
来源：http://efl.tianlin.xyz

Go:   type User struct { Name string; Age int }
来源：http://uoa.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lsr.yj202588.top

C#:   record User(string Name, int Age);
来源：http://wwj.kuanghao11.cn

[G15] 枚举
来源：http://abp.jyoumei.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jlh.redwolf501.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://rfx.chenlongwang.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hdg.dashuyun.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jis.chenjidiqi.icu

Java: enum Color { RED, GREEN }
来源：http://esf.quarkkingdee.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zqy.sufxvd.cn

Ruby: Color = %i[red green].freeze
来源：http://mmj.yj202588.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uvt.yuxming.cn

[G16] 对象转数组 / 字典
来源：http://gxu.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://awb.feifeiyinyue.top

PHP:  get_object_vars($obj);
来源：http://mau.yj202588.top

JS:   Object.entries(obj)
来源：http://xie.dianchejie.cn

TS:   Object.entries(obj)
来源：http://kar.epnwcf.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jbf.guannengcc.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://lzz.meibo888.top

Ruby: obj.instance_variables
来源：http://wwb.sweek.top

C#:   // 用反射或 System.Text.Json
来源：http://rwx.chenzaomai.com

================================================================================
来源：http://tak.iojbl.cn

H. 异常与错误处理
来源：http://efn.hnqzz.top

================================================================================
来源：http://fcc.zhongyouzk.top

[H01] try / catch 基础
来源：http://zuq.jinyuanbaomall.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tje.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iqv.316326.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://knv.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lgi.xingfuxueyuan.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ama.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fsv.ybcxt.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ved.c1oappe.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dhs.ybcxt.top

[H02] finally / ensure 收尾
来源：http://mok.fengsongda.top

Py:   try: f()⏎finally: cleanup()
来源：http://cwj.shangyingyoupin.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://opr.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://owl.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://irx.shanyushiyangkeji.top

Java: try { f(); } finally { cleanup(); }
来源：http://vfx.jianghu66.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jnr.havefunace.top

Ruby: begin; f; ensure; cleanup; end
来源：http://rsf.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vad.nwbrower.top

[H03] 主动抛出异常
来源：http://poj.daxiang520.top

Py:   raise ValueError("错误信息")
来源：http://rfw.ydjk.org.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ujw.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://vvb.fengsongda.top

TS:   throw new Error("错误信息");
来源：http://oaw.zhaomingkeji.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://ydp.zhiwuduotai.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://txm.jinghuilouyu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bip.fktsv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tmf.jinghuilouyu.cn

[H04] 自定义异常类型
来源：http://hud.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://pxa.hfpthk.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qjv.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://rkt.hfpthk.cn

TS:   class MyError extends Error {}
来源：http://mtx.shuidangran.top

Java: class MyException extends RuntimeException {}
来源：http://wzo.sweek.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eod.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://fpb.sufxvd.cn

C#:   class MyException : Exception {}
来源：http://rix.pycfn.com

[H05] 捕获特定类型
来源：http://cri.iojbl.cn

Py:   except ValueError as e:
来源：http://tsy.jqgfzy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cvv.jqgfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://aln.andypj.xyz

TS:   if (e instanceof TypeError) {}
来源：http://reg.jinyuanbaomall.cn

Java: catch (IOException | SQLException e) {}
来源：http://ljn.shanyushiyangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://djq.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://ghg.hcnkem.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bzl.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://zfi.yj20258.top

Py:   value = d.get("k") or default
来源：http://pxw.svipenyu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://utb.xingfuxueyuan.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://gtz.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dbv.nanxinkj.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fpq.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dfy.ywan-chungtsiang.top

Ruby: d&.dig(:a, :b)
来源：http://ice.ybcxt.top

C#:   obj?.A?.B ?? default
来源：http://wrs.jinqigfzy.top

[H07] 断言
来源：http://aak.xuanzx.com

Py:   assert x > 0, "必须为正"
来源：http://pzn.guannengcc.top

PHP:  assert($x > 0);
来源：http://ylb.tarul.cn

JS:   console.assert(x > 0);
来源：http://cgp.aibaodan.cn

TS:   console.assert(x > 0);
来源：http://dqo.pycfn.com

Java: assert x > 0 : "必须为正";
来源：http://qmg.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://knq.ctjpmb.com

Ruby: raise "必须为正" unless x > 0
来源：http://dms.jqgfzy.top

C#:   Debug.Assert(x > 0);
来源：http://yef.dianchejie.cn

[H08] 获取错误信息与堆栈
来源：http://xex.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://fxq.hesvh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yqj.fehbvm.com

JS:   e.message;  e.stack
来源：http://qsu.cqqwz.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tiq.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tdw.fanxiaobao.xyz

Go:   err.Error()
来源：http://byl.hnqzz.top

Ruby: e.message;  e.backtrace
来源：http://nqx.iojbl.cn

C#:   e.Message;  e.StackTrace
来源：http://ezb.nanxuanxn.top

[H09] 带错误码的异常
来源：http://xrj.xuetiantiany.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ksw.cdnleiting.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tjx.9152youxi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ptw.hesvh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fdm.cheryme.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hgy.zdqjudy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ifu.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rje.hnxiangtu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://gsm.chenzaomai.com

[H10] 资源自动释放
来源：http://wzg.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ias.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xud.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://udw.hcnkem.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cvp.sxryk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kir.cashguo.top

Go:   defer f.Close()
来源：http://nom.sxryk.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ymk.bbcook.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mrt.iojbl.cn

================================================================================
来源：http://wft.shuidangran.top

I. 正则表达式
来源：http://fsq.ybcxt.top

================================================================================
来源：http://lcz.jianghu66.top

[I01] 判断是否匹配
来源：http://wfz.havefunace.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hsk.tianlin.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://ihj.aibaodan.cn

JS:   /\d+/.test(s)
来源：http://wbd.xylfe.cn

TS:   /\d+/.test(s)
来源：http://oss.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kzx.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rya.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://mda.316326.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://enb.fktsv.cn

[I02] 提取所有匹配
来源：http://kgi.pycfn.com

Py:   re.findall(r"\d+", s)
来源：http://txg.uphjek.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://per.yuanzhike.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zyl.jqgufenzy.top

TS:   s.match(/\d+/g)
来源：http://xrl.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zck.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bku.tarul.cn

Ruby: s.scan(/\d+/)
来源：http://gtw.hcnkem.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xqw.ivvv.top

[I03] 提取捕获分组
来源：http://jod.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qyl.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uzb.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nin.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mlh.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ipe.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rnm.nanxuanxn.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rxm.dianchejie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gij.chenzaomai.com

[I04] 正则替换
来源：http://sco.zycfv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://eao.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jkv.shzxlz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://egs.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qww.zhiwuduotai.top

Java: s.replaceAll("\\d+", "#")
来源：http://qei.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://akc.shanyushiyangtech.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wqt.chenzaomai.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mox.bbcook.cn

[I05] 按正则拆分
来源：http://amq.snrcjt.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kap.hongshengwenyu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fnv.daxiang520.top

JS:   s.split(/\s*,\s*/)
来源：http://ewg.zhixingplan.top

TS:   s.split(/\s*,\s*/)
来源：http://odi.jiagoushi.top

Java: s.split("\\s*,\\s*")
来源：http://chl.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://moz.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uii.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rfm.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://fkh.yj202588.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdw.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kri.zhaomingkeji.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqc.snrcjt.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://guy.hfpthk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rgf.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ckf.yonumen.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xcp.jinqigfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zrd.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://dsy.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ldw.guowangkeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ksy.andypj.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wtj.yuanzhike.top

TS:   /error/gim
来源：http://kzb.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hjd.quarkkingdee.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fjq.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://vod.nanxinkj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ujy.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://twg.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ife.sxryk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swc.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uhr.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iww.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://syt.shanyushiyangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xfv.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sce.ydzc1.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qwn.havefunace.top

================================================================================
来源：http://ajz.gaohongyu789.top

J. 日期与时间
来源：http://zmy.cdnleiting.top

================================================================================
来源：http://vag.jinqigufen.top

[J01] 获取当前时间
来源：http://xcf.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hqr.bjfxy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kre.yanxiufei.cn

JS:   new Date();  Date.now()
来源：http://gwy.zhijiandao.cn

TS:   new Date();  Date.now()
来源：http://sfp.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://amy.daria6918.cn

Go:   time.Now()
来源：http://wip.chenzaomai.com

Ruby: Time.now
来源：http://cqp.smart0.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://jpd.aizwys.cn

[J02] 格式化输出
来源：http://mxy.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kxx.aizwys.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zbn.hfpthk.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sfi.bjfxy.top

TS:   d.toISOString()
来源：http://lsk.shzxlz.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zsk.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zrx.yj202588.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zkt.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dbd.meibo888.top

[J03] 字符串解析为日期
来源：http://tlk.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vkn.epnwcf.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tak.shanyushiyangtech.top

JS:   new Date("2024-01-02")
来源：http://lef.aibaodan.cn

TS:   new Date("2024-01-02")
来源：http://vsy.zdqjudy.top

Java: LocalDate.parse("2024-01-02")
来源：http://aya.ctjpmb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xhx.yuanzhike.top

Ruby: Date.parse("2024-01-02")
来源：http://azx.yj202588.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mxf.xingfuxueyuan.xyz

[J04] 时间戳与日期互转
来源：http://xnl.sweek.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jfk.tianlin.xyz

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sea.tarul.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qza.tarul.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ibg.uphjek.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tfp.nanxuanxn.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uhp.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jsy.fzhhl.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jrr.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://fdb.sjlbkw.cn

Py:   now + timedelta(days=7)
来源：http://unb.yvedp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xon.zhengqikj.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://onh.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xxv.hysaishi.cn

Java: LocalDate.now().plusDays(7)
来源：http://fdh.gzhubu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gjp.uphjek.com

Ruby: Time.now + 7 * 86400
来源：http://nra.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ihr.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://dph.bbcook.cn

Py:   (end - start).total_seconds()
来源：http://aye.gotoacloud.top

PHP:  $end->diff($start)->days;
来源：http://jmv.zhixingplan.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://odg.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fgm.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://onq.tanke756.top

Go:   end.Sub(start).Hours()
来源：http://txc.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://jwe.ydjk.org.cn

C#:   (end - start).TotalSeconds
来源：http://dzi.ybcxt.top

[J07] 比较两个日期
来源：http://jax.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://jha.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yku.kuanghao11.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oij.jianghu66.top

TS:   d1.getTime() < d2.getTime()
来源：http://tlu.xingfuxueyuan.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dan.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bei.cucudq.cn

Ruby: d1 < d2;  d1 == d2
来源：http://akw.jyoumei.cn


<!-- 参考信息 -->