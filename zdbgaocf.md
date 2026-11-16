代发 wailian999

Ruby: attr_accessor :name
来源：http://zqx.nwbrower.top

C#:   public string Name { get; set; }
来源：http://yhl.dianchejie.cn

[G12] 对象转字符串
来源：http://xiq.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://dhw.hnxiangtu.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://prt.xuanzx.com

JS:   toString() { return this.name; }
来源：http://yxj.nwbrower.top

TS:   toString(): string { return this.name; }
来源：http://mdb.yuanzhike.top

Java: @Override public String toString() { return name; }
来源：http://zoy.fengsongda.top

Go:   func (u User) String() string { return u.Name }
来源：http://wql.ppjwa.cn

Ruby: def to_s; @name; end
来源：http://zqu.ybcxt.top

C#:   public override string ToString() => Name;
来源：http://ifl.yj202588.top

[G13] 判断对象类型
来源：http://nim.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://ykg.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://zre.jiagoushi.top

JS:   u instanceof User
来源：http://fbm.shzxlz.cn

TS:   u instanceof User
来源：http://msq.cqqwz.cn

Java: u instanceof User
来源：http://nqu.yvedp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pwb.yongpay.top

Ruby: u.is_a?(User)
来源：http://oiz.yuxming.cn

C#:   u is User
来源：http://nja.wangdashe.top

[G14] 数据类 / record
来源：http://psk.bjfxy.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gny.nanxuanxn.top

PHP:  // 用 readonly 属性模拟
来源：http://dsp.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pbm.zhixingplan.top

TS:   type User = { name: string; age: number };
来源：http://upd.daxiang520.top

Java: record User(String name, int age) {}
来源：http://zwm.chenlongwang.top

Go:   type User struct { Name string; Age int }
来源：http://nak.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jtr.yuanzhike.top

C#:   record User(string Name, int Age);
来源：http://vnk.shanyushiyangtech.top

[G15] 枚举
来源：http://rol.wangdashe.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pzx.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bjw.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://irn.epnwcf.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mut.fanxiaobao.xyz

Java: enum Color { RED, GREEN }
来源：http://ert.xylfe.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oci.yuanzhike.top

Ruby: Color = %i[red green].freeze
来源：http://gje.chenjidiqi.icu

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rjt.sysykeji.top

[G16] 对象转数组 / 字典
来源：http://wgl.zdbjq.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zkk.shangyingyoupin.top

PHP:  get_object_vars($obj);
来源：http://kzj.yanxiufei.cn

JS:   Object.entries(obj)
来源：http://gsk.chenzaomai.com

TS:   Object.entries(obj)
来源：http://mzs.smart0.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ngh.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fve.gzhubu.top

Ruby: obj.instance_variables
来源：http://sai.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://wga.jianghu66.top

================================================================================
来源：http://jkg.nanxinkj.top

H. 异常与错误处理
来源：http://vbb.gaohongyu789.top

================================================================================
来源：http://ixa.gzhubu.top

[H01] try / catch 基础
来源：http://jwa.svipenyu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jzz.shanyushiyangkeji.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ngs.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pol.xziqi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qrt.shanyushiyangtech.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xod.ydjk.org.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ahk.ydzc1.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nzm.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uey.dashuyun.cn

[H02] finally / ensure 收尾
来源：http://god.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://kps.yfazqb.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://gga.vehdjk.com

JS:   try { f(); } finally { cleanup(); }
来源：http://fea.ppjwa.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://skj.cucudq.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wbs.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ppo.jiagoushi.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ogi.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vmg.hfpthk.cn

[H03] 主动抛出异常
来源：http://yco.hcnkem.com

Py:   raise ValueError("错误信息")
来源：http://vvg.dashuyun.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://okv.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://fey.sufxvd.cn

TS:   throw new Error("错误信息");
来源：http://sus.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://wnk.xinyue.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bma.zdqjudy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ini.chenlongwang.top

C#:   throw new ArgumentException("错误信息");
来源：http://bcy.sjlbkw.cn

[H04] 自定义异常类型
来源：http://jco.zdqjudy.top

Py:   class MyError(Exception): pass
来源：http://vvj.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://dfp.daria6918.cn

JS:   class MyError extends Error {}
来源：http://dpr.shanyushiyangkeji.top

TS:   class MyError extends Error {}
来源：http://hyf.zhixingplan.top

Java: class MyException extends RuntimeException {}
来源：http://eps.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bhk.epnwcf.com

Ruby: class MyError < StandardError; end
来源：http://hgg.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://amb.ctjpmb.com

[H05] 捕获特定类型
来源：http://phy.shuidangran.top

Py:   except ValueError as e:
来源：http://fen.xingfuxueyuan.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ami.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://fck.jyoumei.cn

TS:   if (e instanceof TypeError) {}
来源：http://whd.zycfv.cn

Java: catch (IOException | SQLException e) {}
来源：http://uxv.sxryk.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zec.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://jbo.ydjk.org.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lme.xylfe.cn

[H06] 可选值 / 空值安全访问
来源：http://aks.ppjwa.cn

Py:   value = d.get("k") or default
来源：http://ydp.gaohongyu789.top

PHP:  $v = $d["k"] ?? null;
来源：http://kor.chenjidiqi.icu

JS:   obj?.a?.b;  d ?? default
来源：http://yam.chenzaomai.com

TS:   obj?.a?.b;  d ?? default
来源：http://qbs.vehdjk.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kwv.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://var.ydjk.org.cn

Ruby: d&.dig(:a, :b)
来源：http://rdw.snrcjt.cn

C#:   obj?.A?.B ?? default
来源：http://lwa.zhoulong.xyz

[H07] 断言
来源：http://ogj.smart0.xyz

Py:   assert x > 0, "必须为正"
来源：http://mnh.guowangkeji.top

PHP:  assert($x > 0);
来源：http://wyf.ppjwa.cn

JS:   console.assert(x > 0);
来源：http://ubl.hammf.cn

TS:   console.assert(x > 0);
来源：http://mha.chenlongwang.top

Java: assert x > 0 : "必须为正";
来源：http://jhx.zdbjq.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bui.zhaomingkeji.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://xwj.yangfankeji.com

C#:   Debug.Assert(x > 0);
来源：http://kbm.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://irc.cqqwz.cn

Py:   str(e);  traceback.format_exc()
来源：http://pjc.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wbz.zhixingplan.top

JS:   e.message;  e.stack
来源：http://suy.xinyue.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://spp.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ctj.nwbrower.top

Go:   err.Error()
来源：http://wuz.shanyushiyangkeji.top

Ruby: e.message;  e.backtrace
来源：http://cyw.ydjk.org.cn

C#:   e.Message;  e.StackTrace
来源：http://rcn.meibo888.top

[H09] 带错误码的异常
来源：http://sfh.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tjz.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jen.dianchejie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hxk.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ndl.nanxinkj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sju.redwolf501.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mdl.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bqk.yuxming.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ygw.yongpay.top

[H10] 资源自动释放
来源：http://qll.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ywr.jianghu66.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ewp.yangfankeji.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yuk.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aol.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xpz.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://fmz.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ynq.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zco.yfazqb.com

================================================================================
来源：http://wkj.ivvv.top

I. 正则表达式
来源：http://twr.wangdashe.top

================================================================================
来源：http://phz.ctjpmb.com

[I01] 判断是否匹配
来源：http://izo.bbcook.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cpl.jinghuilouyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gca.sweek.top

JS:   /\d+/.test(s)
来源：http://vmg.316326.xyz

TS:   /\d+/.test(s)
来源：http://osw.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cxt.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://msi.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://cgz.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xdq.hysaishi.cn

[I02] 提取所有匹配
来源：http://qsh.jlsjyb.cn

Py:   re.findall(r"\d+", s)
来源：http://mba.zycfv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xlj.shuidangran.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gnj.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://evd.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mqc.sjlbkw.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kdc.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://fpr.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iky.tian-w.cn

[I03] 提取捕获分组
来源：http://jav.iojbl.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xxq.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rjh.guowangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ges.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gyj.yangfankeji.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sxb.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eqr.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://azp.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oby.gotoacloud.top

[I04] 正则替换
来源：http://irj.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://uoy.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ozm.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lcz.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://mit.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://bdt.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://whh.tianlin.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://wpu.aizwys.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://szj.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://sxx.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://fib.yj20258.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wyt.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://dni.yangfankeji.com

TS:   s.split(/\s*,\s*/)
来源：http://ofp.uphjek.com

Java: s.split("\\s*,\\s*")
来源：http://njg.chenlongwang.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vpd.mhx1999.top

Ruby: s.split(/\s*,\s*/)
来源：http://qrg.9152youxi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jca.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://llq.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bdu.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rrn.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://myo.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tpt.ydjk.org.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eeq.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rbg.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://inx.ywan-chungtsiang.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yfs.guowangkeji.top

[I07] 忽略大小写与多行模式
来源：http://mlw.yuanzhike.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hpa.gotoacloud.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ene.0kj1m.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wzx.meibo888.top

TS:   /error/gim
来源：http://jcr.gzhubu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mly.shanyushiyangkeji.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zgf.xingfuxueyuan.xyz

Ruby: s.scan(/error/i)
来源：http://tjb.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wtc.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://qhr.ctjpmb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://duq.316326.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rzp.hesvh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xng.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://onu.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rto.yonumen.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rfx.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tyi.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lqk.jiagoushi.top

================================================================================
来源：http://mma.hammf.cn

J. 日期与时间
来源：http://psv.hysaishi.cn

================================================================================
来源：http://wsu.9152youxi.cn

[J01] 获取当前时间
来源：http://rhd.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://glv.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rix.daxiang520.top

JS:   new Date();  Date.now()
来源：http://qkk.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://wyn.zycfv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eiw.bjfxy.top

Go:   time.Now()
来源：http://lac.yuanzhike.top

Ruby: Time.now
来源：http://wgz.fengsongda.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cyo.yangfankeji.com

[J02] 格式化输出
来源：http://wsv.zhoulong.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://spi.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dgd.nanxuanxn.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://npi.jlsjyb.cn

TS:   d.toISOString()
来源：http://omu.epnwcf.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fst.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iue.jiagoushi.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://svk.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yyz.aizwys.cn

[J03] 字符串解析为日期
来源：http://fui.gzhubu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fqv.xylfe.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rov.aibaodan.cn

JS:   new Date("2024-01-02")
来源：http://ngy.andypj.xyz

TS:   new Date("2024-01-02")
来源：http://xlj.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zqe.hfpthk.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rup.havefunace.top

Ruby: Date.parse("2024-01-02")
来源：http://pbu.ybcxt.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qyt.tanke756.top

[J04] 时间戳与日期互转
来源：http://nee.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vyr.nwbrower.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xks.guannengcc.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cly.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vrh.nanxuanxn.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qdn.fengsongda.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://aaz.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tkb.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nqv.jyoumei.cn

[J05] 时间加减（加 7 天）
来源：http://oth.ehwqpu.com

Py:   now + timedelta(days=7)
来源：http://ilr.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://ufg.shanyushiyangtech.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sed.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cbx.jyoumei.cn

Java: LocalDate.now().plusDays(7)
来源：http://lwj.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iij.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://eng.xingfuxueyuan.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://cyp.wangdashe.top

[J06] 计算两时间之差
来源：http://irw.yj202588.top

Py:   (end - start).total_seconds()
来源：http://tpd.uphjek.com

PHP:  $end->diff($start)->days;
来源：http://ztf.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://evb.feifeiyinyue.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cjw.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ngp.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://dpq.svipenyu.cn

Ruby: end - start                 # 返回秒数
来源：http://hzt.xuanzx.com

C#:   (end - start).TotalSeconds
来源：http://lxg.zhoulong.xyz

[J07] 比较两个日期
来源：http://hyh.yanxiufei.cn

Py:   d1 < d2;  d1 == d2
来源：http://dkk.zhijiandao.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xcj.svipenyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://igu.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://uol.feifeiyinyue.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cll.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jwr.chenzaomai.com

Ruby: d1 < d2;  d1 == d2
来源：http://jyc.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://abw.snrcjt.cn

[J08] 提取年月日与星期
来源：http://wxt.316326.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nyt.birdmap.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hqp.cheryme.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gcl.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xrt.fzhhl.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rzx.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qtq.shangyingyoupin.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kge.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fdy.yvedp.cn

[J09] 时区处理
来源：http://sgr.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fid.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://udl.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://exh.yj202588.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rzd.fanxiaobao.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dcz.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://spd.yongpay.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ovx.vqdsnc.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yub.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://swl.andypj.xyz


<!-- 参考信息 -->