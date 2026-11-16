代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://lby.andypj.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://ykx.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ftn.nanxinkj.top

TS:   interface Shape { area(): number; }
来源：http://iav.bjfxy.top

Java: interface Shape { double area(); }
来源：http://lzs.dianchejie.cn

Go:   type Shape interface { Area() float64 }
来源：http://mtc.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cfq.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://bct.cheryme.top

[G10] 访问控制
来源：http://znc.yongpay.top

Py:   约定 _protected / __private（不强制）
来源：http://kmm.jianghu66.top

PHP:  public / protected / private
来源：http://fxl.aizwys.cn

JS:   #private 字段；其余公开
来源：http://tcs.chenlongwang.top

TS:   public / protected / private
来源：http://riq.zhiwuduotai.top

Java: public / protected / private / 默认包级
来源：http://lti.svipenyu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gzy.yfazqb.com

Ruby: public / protected / private
来源：http://mhu.chenjidiqi.icu

C#:   public / protected / private / internal
来源：http://qku.xziqi.cn

[G11] getter / setter
来源：http://dek.daria6918.cn

Py:   @property 与 @x.setter
来源：http://wwy.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pbl.chenzaomai.com

JS:   get name() { return this._name; }
来源：http://kcj.hnxiangtu.top

TS:   get name(): string { return this._name; }
来源：http://agx.chenzaomai.com

Java: public String getName() { return name; }
来源：http://yxl.shzxlz.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bvr.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://ctu.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://idm.zycfv.cn

[G12] 对象转字符串
来源：http://cdn.cashguo.top

Py:   def __str__(self): return self.name
来源：http://rij.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://onz.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://gtl.xuetiantiany.cn

TS:   toString(): string { return this.name; }
来源：http://vwn.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://jte.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://ahb.shangyingyoupin.top

Ruby: def to_s; @name; end
来源：http://gtv.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://bvm.hammf.cn

[G13] 判断对象类型
来源：http://lsq.guannengcc.top

Py:   isinstance(u, User)
来源：http://szn.c1oappe.top

PHP:  $u instanceof User
来源：http://ife.ppjwa.cn

JS:   u instanceof User
来源：http://fxy.zhengqikj.top

TS:   u instanceof User
来源：http://apc.chenjidiqi.icu

Java: u instanceof User
来源：http://pwt.gogol.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fbo.feifeiyinyue.top

Ruby: u.is_a?(User)
来源：http://wjk.9152youxi.cn

C#:   u is User
来源：http://ogr.zhengqikj.top

[G14] 数据类 / record
来源：http://wlh.meibo888.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://usd.chenjidiqi.icu

PHP:  // 用 readonly 属性模拟
来源：http://gql.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kty.sjlbkw.cn

TS:   type User = { name: string; age: number };
来源：http://kjj.ydjk.org.cn

Java: record User(String name, int age) {}
来源：http://vsv.gotoacloud.top

Go:   type User struct { Name string; Age int }
来源：http://woi.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aah.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://rge.yvedp.cn

[G15] 枚举
来源：http://drb.yuxming.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lcl.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://crc.guannengcc.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qek.xinyue.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://del.zhaomingkeji.xyz

Java: enum Color { RED, GREEN }
来源：http://sau.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://odj.jinqigfzy.top

Ruby: Color = %i[red green].freeze
来源：http://hkv.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://spg.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://qwh.cashguo.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dbp.cucudq.cn

PHP:  get_object_vars($obj);
来源：http://dze.shanyushiyangtech.top

JS:   Object.entries(obj)
来源：http://aei.svipenyu.cn

TS:   Object.entries(obj)
来源：http://mmd.tian-w.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wpq.yangfankeji.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://mbn.zhaomingkeji.xyz

Ruby: obj.instance_variables
来源：http://smt.dashuyun.cn

C#:   // 用反射或 System.Text.Json
来源：http://hsj.fktsv.cn

================================================================================
来源：http://mjl.sxryk.cn

H. 异常与错误处理
来源：http://uwl.smart0.xyz

================================================================================
来源：http://shb.yonumen.top

[H01] try / catch 基础
来源：http://bqp.xingfuxueyuan.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gqg.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ogk.bbcook.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://irf.dashuyun.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ufc.nanxuanxn.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xtg.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oiv.0kj1m.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://upb.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kbx.kuanghao11.cn

[H02] finally / ensure 收尾
来源：http://wgg.jlsjyb.cn

Py:   try: f()⏎finally: cleanup()
来源：http://avx.jinqigufen.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rkl.aibaodan.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://msi.cucudq.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fqv.smart0.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://hdu.snrcjt.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ygl.zhiwuduotai.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vuq.fanxiaobao.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://ewa.yuanzhike.top

[H03] 主动抛出异常
来源：http://qnl.aibaodan.cn

Py:   raise ValueError("错误信息")
来源：http://zzd.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gcv.fzhhl.top

JS:   throw new Error("错误信息");
来源：http://apk.hfpthk.cn

TS:   throw new Error("错误信息");
来源：http://wcj.bjfxy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wcg.kuanghao11.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ori.gogol.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wvv.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dif.ehwqpu.com

[H04] 自定义异常类型
来源：http://krf.vqdsnc.cn

Py:   class MyError(Exception): pass
来源：http://usn.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rqq.yonumen.top

JS:   class MyError extends Error {}
来源：http://wsu.tian-w.cn

TS:   class MyError extends Error {}
来源：http://rkb.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://rvv.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xav.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://bye.gotoacloud.top

C#:   class MyException : Exception {}
来源：http://rkq.cashguo.top

[H05] 捕获特定类型
来源：http://xfl.ivvv.top

Py:   except ValueError as e:
来源：http://fah.fengsongda.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zje.andypj.xyz

JS:   if (e instanceof TypeError) {}
来源：http://gua.sweek.top

TS:   if (e instanceof TypeError) {}
来源：http://zkc.redwolf501.top

Java: catch (IOException | SQLException e) {}
来源：http://hip.guannengcc.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gkg.shanyushiyangtech.top

Ruby: rescue ArgumentError => e
来源：http://hxe.jyoumei.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lkv.yuxming.cn

[H06] 可选值 / 空值安全访问
来源：http://qzd.yfazqb.com

Py:   value = d.get("k") or default
来源：http://jab.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://prs.shuidangran.top

JS:   obj?.a?.b;  d ?? default
来源：http://rye.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rpu.bjfxy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://goa.xylfe.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://htu.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://sca.pengpengdd.cyou

C#:   obj?.A?.B ?? default
来源：http://ohx.sysykeji.top

[H07] 断言
来源：http://hal.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://xsy.snrcjt.cn

PHP:  assert($x > 0);
来源：http://bpi.xylfe.cn

JS:   console.assert(x > 0);
来源：http://dos.nwbrower.top

TS:   console.assert(x > 0);
来源：http://axc.cdnleiting.top

Java: assert x > 0 : "必须为正";
来源：http://dda.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ijz.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hgr.chenzaomai.com

C#:   Debug.Assert(x > 0);
来源：http://gja.jinyuanbaomall.cn

[H08] 获取错误信息与堆栈
来源：http://jlv.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://kfi.bjfxy.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wwn.cqqwz.cn

JS:   e.message;  e.stack
来源：http://hvl.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hef.yfazqb.com

Java: e.getMessage();  e.printStackTrace()
来源：http://haw.nanxuanxn.top

Go:   err.Error()
来源：http://sle.chenzaomai.com

Ruby: e.message;  e.backtrace
来源：http://bni.hammf.cn

C#:   e.Message;  e.StackTrace
来源：http://dit.wangdashe.top

[H09] 带错误码的异常
来源：http://hbq.jianghu66.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://obw.epnwcf.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://odk.316326.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wtk.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kft.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tly.snrcjt.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://win.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iyt.cheryme.top

C#:   // 自定义异常类中加 Code 属性
来源：http://rix.havefunace.top

[H10] 资源自动释放
来源：http://zrh.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mon.aibaodan.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sub.gotoacloud.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xbw.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fkf.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://phj.tian-w.cn

Go:   defer f.Close()
来源：http://qjf.bbcook.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://umh.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://aio.hnxiangtu.top

================================================================================
来源：http://xuh.xziqi.cn

I. 正则表达式
来源：http://mli.bbcook.cn

================================================================================
来源：http://olv.ydjk.org.cn

[I01] 判断是否匹配
来源：http://ceo.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wbo.fktsv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://psa.yvedp.cn

JS:   /\d+/.test(s)
来源：http://gsh.yfazqb.com

TS:   /\d+/.test(s)
来源：http://lcu.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rdm.kuanghao11.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://acy.vehdjk.com

Ruby: s.match?(/\d+/)
来源：http://nur.snrcjt.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vpz.hesvh.cn

[I02] 提取所有匹配
来源：http://xju.vqdsnc.cn

Py:   re.findall(r"\d+", s)
来源：http://kcc.chenzaomai.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rkd.zhijiandao.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gus.xuanzx.com

TS:   s.match(/\d+/g)
来源：http://cno.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qwk.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nxc.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://avd.uphjek.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kmq.zhongyouzk.top

[I03] 提取捕获分组
来源：http://zxe.hcnkem.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gmj.snrcjt.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wwi.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qnb.iojbl.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yze.sysykeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ekv.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pjo.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lzh.ehwqpu.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nlq.yonumen.top

[I04] 正则替换
来源：http://qiu.jinyuanbaomall.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gzz.tarul.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://riq.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://meb.nwbrower.top

TS:   s.replace(/\d+/g, "#")
来源：http://bgi.wangdashe.top

Java: s.replaceAll("\\d+", "#")
来源：http://jzj.ctjpmb.com

Go:   re.ReplaceAllString(s, "#")
来源：http://dsz.birdmap.top

Ruby: s.gsub(/\d+/, "#")
来源：http://cik.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uhc.andypj.xyz

[I05] 按正则拆分
来源：http://aqu.yonumen.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hak.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://izo.cqqwz.cn

JS:   s.split(/\s*,\s*/)
来源：http://rsx.jqgufenzy.top

TS:   s.split(/\s*,\s*/)
来源：http://ejv.tanke756.top

Java: s.split("\\s*,\\s*")
来源：http://mji.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zek.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://tbg.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cio.feifeiyinyue.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pat.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pxa.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://npr.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bgo.pycfn.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvb.sxryk.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xqz.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://atc.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fgk.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gxv.zhijiandao.cn

[I07] 忽略大小写与多行模式
来源：http://boa.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://osi.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://olj.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kyx.sjlbkw.cn

TS:   /error/gim
来源：http://awr.yj202588.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://per.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qmf.yueranfly.top

Ruby: s.scan(/error/i)
来源：http://fif.zhongyouzk.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fnq.wangshuangyany.cn

[I08] 贪婪与非贪婪匹配
来源：http://lac.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nnf.meibo888.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wea.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mks.pengpengdd.cyou

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://auq.zdbjq.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tqq.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pcm.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jxc.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bth.0kj1m.cn

================================================================================
来源：http://uzw.ctjpmb.com

J. 日期与时间
来源：http://ium.fktsv.cn

================================================================================
来源：http://nyh.cqqwz.cn

[J01] 获取当前时间
来源：http://ran.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://asj.gotoacloud.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tsu.aizwys.cn

JS:   new Date();  Date.now()
来源：http://rkc.ctjpmb.com

TS:   new Date();  Date.now()
来源：http://cpo.dashuyun.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wys.sysykeji.top

Go:   time.Now()
来源：http://jzm.tanke756.top

Ruby: Time.now
来源：http://yfh.jinqigufen.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ihx.snrcjt.cn

[J02] 格式化输出
来源：http://zvo.cashguo.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://txf.jlsjyb.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vsu.jqgufenzy.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ohw.epnwcf.com

TS:   d.toISOString()
来源：http://ttw.gogol.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xom.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://naj.iojbl.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nip.xziqi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hkh.tarul.cn

[J03] 字符串解析为日期
来源：http://ubk.jqgfzy.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ssp.jiagoushi.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uqh.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://dov.xziqi.cn

TS:   new Date("2024-01-02")
来源：http://xbx.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://ggq.snrcjt.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wpa.pengpengdd.cyou

Ruby: Date.parse("2024-01-02")
来源：http://iol.shzxlz.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hka.chenjidiqi.icu

[J04] 时间戳与日期互转
来源：http://vae.yueranfly.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://muv.pycfn.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xij.tanke756.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hue.chenzaomai.com

TS:   Math.floor(Date.now() / 1000)
来源：http://rts.yfazqb.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://tym.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ymq.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xzd.yfazqb.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bhs.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://ndl.yj20258888.top

Py:   now + timedelta(days=7)
来源：http://olo.0kj1m.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oph.jinghuilouyu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://toz.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tkl.yueranfly.top

Java: LocalDate.now().plusDays(7)
来源：http://yil.chenjidiqi.icu

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oev.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://vbm.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gfu.iojbl.cn

[J06] 计算两时间之差
来源：http://gxv.zhiwuduotai.top

Py:   (end - start).total_seconds()
来源：http://zxt.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://eed.jinqigufen.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://azh.zhixingplan.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://oaz.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://psf.hongshengwenyu.top

Go:   end.Sub(start).Hours()
来源：http://erz.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://tjk.pengpengdd.cyou

C#:   (end - start).TotalSeconds
来源：http://elx.jianghu66.top

[J07] 比较两个日期
来源：http://oga.yvedp.cn

Py:   d1 < d2;  d1 == d2
来源：http://ejp.yongpay.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://znx.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://egf.yj20258.top


<!-- 参考信息 -->