代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://uld.jinyuanbaomall.cn

Ruby: def to_s; @name; end
来源：http://zlr.jinyuanbaomall.cn

C#:   public override string ToString() => Name;
来源：http://gyj.shanyushiyangtech.top

[G13] 判断对象类型
来源：http://xgh.zhengqikj.top

Py:   isinstance(u, User)
来源：http://vyu.tianlin.xyz

PHP:  $u instanceof User
来源：http://yiu.haohaochexian.top

JS:   u instanceof User
来源：http://gtc.sysykeji.top

TS:   u instanceof User
来源：http://eus.quarkkingdee.top

Java: u instanceof User
来源：http://uke.0kj1m.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hdx.jyoumei.cn

Ruby: u.is_a?(User)
来源：http://oqv.tarul.cn

C#:   u is User
来源：http://wrt.zhongyouzk.top

[G14] 数据类 / record
来源：http://qqy.guowangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kat.jianghu66.top

PHP:  // 用 readonly 属性模拟
来源：http://dws.ctjpmb.com

JS:   // 无内置：普通类或对象字面量
来源：http://cyl.hysaishi.cn

TS:   type User = { name: string; age: number };
来源：http://mev.316326.xyz

Java: record User(String name, int age) {}
来源：http://qhp.guowangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://lli.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bqh.fehbvm.com

C#:   record User(string Name, int Age);
来源：http://wnp.daria6918.cn

[G15] 枚举
来源：http://fhj.ywan-chungtsiang.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vro.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://clp.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gig.sufxvd.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gwp.ydzc1.top

Java: enum Color { RED, GREEN }
来源：http://daf.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zay.xylfe.cn

Ruby: Color = %i[red green].freeze
来源：http://dzd.mhx1999.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rlp.uphjek.com

[G16] 对象转数组 / 字典
来源：http://dra.cdnleiting.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zxm.tanke756.top

PHP:  get_object_vars($obj);
来源：http://vwv.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://rgl.zhoulong.xyz

TS:   Object.entries(obj)
来源：http://fln.nanxinkj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vim.jqgufenzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://twe.cheryme.top

Ruby: obj.instance_variables
来源：http://rrv.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://lnh.bbcook.cn

================================================================================
来源：http://drw.zhongyouzk.top

H. 异常与错误处理
来源：http://onv.uphjek.com

================================================================================
来源：http://czk.tianlin.xyz

[H01] try / catch 基础
来源：http://svd.pycfn.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ssp.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fyt.gzhubu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ipu.fktsv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zjr.birdmap.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vrz.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lnu.nanxuanxn.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eqj.nanxinkj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ifi.sxryk.cn

[H02] finally / ensure 收尾
来源：http://rnq.haohaochexian.top

Py:   try: f()⏎finally: cleanup()
来源：http://mlz.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://xrc.yj202588.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qfx.nanxuanxn.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ftj.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lmt.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://zob.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://frd.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oct.xylfe.cn

[H03] 主动抛出异常
来源：http://etc.yvedp.cn

Py:   raise ValueError("错误信息")
来源：http://zja.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gbh.yj20258888.top

JS:   throw new Error("错误信息");
来源：http://ibq.fehbvm.com

TS:   throw new Error("错误信息");
来源：http://iiz.shangyingyoupin.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://nzx.c1oappe.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://deg.wangshuangyany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vhj.gaohongyu789.top

C#:   throw new ArgumentException("错误信息");
来源：http://jko.ppjwa.cn

[H04] 自定义异常类型
来源：http://fqa.nwbrower.top

Py:   class MyError(Exception): pass
来源：http://rry.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://vad.mhx1999.top

JS:   class MyError extends Error {}
来源：http://dnd.zhixingplan.top

TS:   class MyError extends Error {}
来源：http://jyc.jlsjyb.cn

Java: class MyException extends RuntimeException {}
来源：http://qsx.cucudq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pyb.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://mpe.ybcxt.top

C#:   class MyException : Exception {}
来源：http://rbt.zycfv.cn

[H05] 捕获特定类型
来源：http://moh.tian-w.cn

Py:   except ValueError as e:
来源：http://mey.yj20258888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wdv.jinghuilouyu.cn

JS:   if (e instanceof TypeError) {}
来源：http://swz.kuanghao11.cn

TS:   if (e instanceof TypeError) {}
来源：http://afb.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://qqq.52xcode.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fda.zhiwuduotai.top

Ruby: rescue ArgumentError => e
来源：http://hgn.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hrb.jianghu66.top

[H06] 可选值 / 空值安全访问
来源：http://ulw.cheryme.top

Py:   value = d.get("k") or default
来源：http://djn.yvedp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lkp.havefunace.top

JS:   obj?.a?.b;  d ?? default
来源：http://rxl.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://ftb.xuanzx.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gtp.bjfxy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://xyj.hcnkem.com

Ruby: d&.dig(:a, :b)
来源：http://rmf.zhixingplan.top

C#:   obj?.A?.B ?? default
来源：http://soj.shanyushiyangkeji.top

[H07] 断言
来源：http://rpg.yanxiufei.cn

Py:   assert x > 0, "必须为正"
来源：http://qmz.ctjpmb.com

PHP:  assert($x > 0);
来源：http://ukb.cqqwz.cn

JS:   console.assert(x > 0);
来源：http://myn.xuetiantiany.cn

TS:   console.assert(x > 0);
来源：http://wxt.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://zbi.0kj1m.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jnk.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://prf.smart0.xyz

C#:   Debug.Assert(x > 0);
来源：http://nee.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://cry.svipenyu.cn

Py:   str(e);  traceback.format_exc()
来源：http://btu.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yaf.bjfxy.top

JS:   e.message;  e.stack
来源：http://lsp.dianchejie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jyj.xinyue.icu

Java: e.getMessage();  e.printStackTrace()
来源：http://zyn.redwolf501.top

Go:   err.Error()
来源：http://wul.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://npu.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://tpf.hywenlv.cn

[H09] 带错误码的异常
来源：http://sue.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gzp.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ccc.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hhi.cqqwz.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uhb.sxryk.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://efr.fzhhl.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dkr.shanyushiyangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://paw.c1oappe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://uzn.chenzaomai.com

[H10] 资源自动释放
来源：http://jkz.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://xfy.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qmx.aizwys.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oke.jlsjyb.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eoq.zdqjudy.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gau.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://egc.hcnkem.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://shx.pycfn.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hfw.fengsongda.top

================================================================================
来源：http://qwq.jqgufenzy.top

I. 正则表达式
来源：http://ady.ydzc1.top

================================================================================
来源：http://wtl.jinqigufen.top

[I01] 判断是否匹配
来源：http://hxe.dashuyun.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bzp.cucudq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qtk.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://ckh.gzhubu.top

TS:   /\d+/.test(s)
来源：http://qoz.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kcl.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jjr.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://gyi.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kci.xylfe.cn

[I02] 提取所有匹配
来源：http://cuv.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://apg.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ncn.ywan-chungtsiang.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vfs.ybcxt.top

TS:   s.match(/\d+/g)
来源：http://egd.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cod.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://btz.zhijiandao.cn

Ruby: s.scan(/\d+/)
来源：http://xyd.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sid.vehdjk.com

[I03] 提取捕获分组
来源：http://biu.chenzaomai.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nyx.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://smh.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rlt.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lwm.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://upq.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wxk.dashuyun.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cug.haohaochexian.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ung.52xcode.cn

[I04] 正则替换
来源：http://goa.zdqjudy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jsz.xuanzx.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://azb.bjfxy.top

JS:   s.replace(/\d+/g, "#")
来源：http://gzn.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gjq.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pcx.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://gaz.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://irv.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rum.hnqzz.top

[I05] 按正则拆分
来源：http://igx.jqgufenzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://qte.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://faq.pengpengdd.cyou

JS:   s.split(/\s*,\s*/)
来源：http://mqm.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://hxk.birdmap.top

Java: s.split("\\s*,\\s*")
来源：http://dyl.yfazqb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vzb.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://viz.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aze.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kjx.sweek.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nad.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dex.birdmap.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvi.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zjz.dashuyun.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://npz.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qtp.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://son.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sts.hongshengwenyu.top

[I07] 忽略大小写与多行模式
来源：http://ejv.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ctb.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zso.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ydm.iojbl.cn

TS:   /error/gim
来源：http://ydf.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zdb.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ipy.ppjwa.cn

Ruby: s.scan(/error/i)
来源：http://ikd.feifeiyinyue.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hkj.yongpay.top

[I08] 贪婪与非贪婪匹配
来源：http://vnb.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zkc.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sdk.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kwa.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pff.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://pwb.wangdashe.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vth.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zya.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://egl.daria6918.cn

================================================================================
来源：http://lcd.sxryk.cn

J. 日期与时间
来源：http://iyx.daxiang520.top

================================================================================
来源：http://spk.gogol.net.cn

[J01] 获取当前时间
来源：http://abz.chenzaomai.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://plu.fengsongda.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zui.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://irn.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://ouw.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://szj.ybcxt.top

Go:   time.Now()
来源：http://aoo.epnwcf.com

Ruby: Time.now
来源：http://geu.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hcq.yvedp.cn

[J02] 格式化输出
来源：http://aqq.dianchejie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jjn.jinyuanbaomall.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wee.tanke756.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pnz.gaohongyu789.top

TS:   d.toISOString()
来源：http://jrz.316326.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eei.ydjk.org.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jrg.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://akk.vehdjk.com

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ttf.cashguo.top

[J03] 字符串解析为日期
来源：http://ryk.zhiwuduotai.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jcq.yuanzhike.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nja.jlsjyb.cn

JS:   new Date("2024-01-02")
来源：http://nnv.yuanzhike.top

TS:   new Date("2024-01-02")
来源：http://ine.ywan-chungtsiang.top

Java: LocalDate.parse("2024-01-02")
来源：http://cnj.yangfankeji.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://omj.ydzc1.top

Ruby: Date.parse("2024-01-02")
来源：http://mhn.dianchejie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://chk.zhaomingkeji.xyz

[J04] 时间戳与日期互转
来源：http://fef.smart0.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bkr.vehdjk.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vth.ydjk.org.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dnb.jinghuilouyu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wic.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ewj.hammf.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rrs.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://urd.jqgfzy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qbq.ydzc1.top

[J05] 时间加减（加 7 天）
来源：http://gtw.gogol.net.cn

Py:   now + timedelta(days=7)
来源：http://tkh.gaohongyu789.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://csj.cqqwz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pzi.sxryk.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqa.guowangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://pcg.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wiy.c1oappe.top

Ruby: Time.now + 7 * 86400
来源：http://gde.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://eoq.hnxiangtu.top

[J06] 计算两时间之差
来源：http://kut.316326.xyz

Py:   (end - start).total_seconds()
来源：http://cor.shanyushiyangkeji.top

PHP:  $end->diff($start)->days;
来源：http://vhz.yj20258.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ksq.hnxiangtu.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xqg.epnwcf.com

Java: Duration.between(start, end).toSeconds()
来源：http://oix.haohaochexian.top

Go:   end.Sub(start).Hours()
来源：http://jax.hywenlv.cn

Ruby: end - start                 # 返回秒数
来源：http://vvr.xziqi.cn

C#:   (end - start).TotalSeconds
来源：http://ita.fktsv.cn

[J07] 比较两个日期
来源：http://bas.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://wcs.gotoacloud.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://awg.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://vnl.kuanghao11.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ddm.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dxd.hesvh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qpd.jinyuanbaomall.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cie.cheryme.top

C#:   d1 < d2;  d1 == d2
来源：http://abm.xziqi.cn

[J08] 提取年月日与星期
来源：http://gtm.sufxvd.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://goo.tianlin.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gpk.svipenyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://elx.fanxiaobao.xyz

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dtg.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dey.hcnkem.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ayx.yuxming.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xhs.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hxr.sysykeji.top

[J09] 时区处理
来源：http://ccz.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zsu.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oyw.jinyuanbaomall.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xtw.zhengqikj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ucg.zdbjq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rpu.chenjidiqi.icu

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bmu.xinyue.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://xlv.zhijiandao.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wbm.sjlbkw.cn

[J10] 取今天 / 本月第一天
来源：http://kag.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gst.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dji.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://anx.yj20258.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sjb.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kcu.vqdsnc.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tjf.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xha.fktsv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hwk.svipenyu.cn


<!-- 参考信息 -->