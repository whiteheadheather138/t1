代发 wailian999

Py:   isinstance(u, User)
来源：http://xrv.zhixingplan.top

PHP:  $u instanceof User
来源：http://uih.zhaomingkeji.xyz

JS:   u instanceof User
来源：http://yod.xuanzx.com

TS:   u instanceof User
来源：http://gdj.guannengcc.top

Java: u instanceof User
来源：http://tmp.zycfv.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://njg.yuanzhike.top

Ruby: u.is_a?(User)
来源：http://kfo.hnxiangtu.top

C#:   u is User
来源：http://uwd.shzxlz.cn

[G14] 数据类 / record
来源：http://nng.daxiang520.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wdc.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://cdz.dashuyun.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uij.shuidangran.top

TS:   type User = { name: string; age: number };
来源：http://cce.nwbrower.top

Java: record User(String name, int age) {}
来源：http://qzv.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://xpq.jqgufenzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cih.tianlin.xyz

C#:   record User(string Name, int Age);
来源：http://dkg.cdnleiting.top

[G15] 枚举
来源：http://zrg.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vmj.jqgufenzy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://otj.ivvv.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ufo.redwolf501.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vgz.xuetiantiany.cn

Java: enum Color { RED, GREEN }
来源：http://xbz.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yrx.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://ihp.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uaj.quarkkingdee.top

[G16] 对象转数组 / 字典
来源：http://jgm.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pun.316326.xyz

PHP:  get_object_vars($obj);
来源：http://pua.jqgfzy.top

JS:   Object.entries(obj)
来源：http://pqq.hysaishi.cn

TS:   Object.entries(obj)
来源：http://wsc.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nex.ydjk.org.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nnt.meibo888.top

Ruby: obj.instance_variables
来源：http://qkm.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://ynd.guannengcc.top

================================================================================
来源：http://dgx.cdnleiting.top

H. 异常与错误处理
来源：http://snj.pycfn.com

================================================================================
来源：http://mai.jinghuilouyu.cn

[H01] try / catch 基础
来源：http://wun.gzhubu.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tru.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lvq.vehdjk.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vwu.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xbl.sjlbkw.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://duv.uphjek.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dek.hesvh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://grn.hcnkem.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://weg.zhaomingkeji.xyz

[H02] finally / ensure 收尾
来源：http://ofa.pengpengdd.cyou

Py:   try: f()⏎finally: cleanup()
来源：http://gsp.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://tdn.shzxlz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aqn.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cqn.cqqwz.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xgo.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tkg.yanxiufei.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sfg.zhiwuduotai.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://blr.hnqzz.top

[H03] 主动抛出异常
来源：http://ipt.nwbrower.top

Py:   raise ValueError("错误信息")
来源：http://wsn.fzhhl.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://udc.zhengqikj.top

JS:   throw new Error("错误信息");
来源：http://ubi.yj202588.top

TS:   throw new Error("错误信息");
来源：http://mzn.yueranfly.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xqr.316326.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hgy.sufxvd.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jfh.meibo888.top

C#:   throw new ArgumentException("错误信息");
来源：http://voh.pengpengdd.cyou

[H04] 自定义异常类型
来源：http://odw.0kj1m.cn

Py:   class MyError(Exception): pass
来源：http://nix.sjlbkw.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ddy.sweek.top

JS:   class MyError extends Error {}
来源：http://bjw.fktsv.cn

TS:   class MyError extends Error {}
来源：http://krs.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://jwo.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hmp.aizwys.cn

Ruby: class MyError < StandardError; end
来源：http://nny.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://jyk.ydjk.org.cn

[H05] 捕获特定类型
来源：http://lpa.xuanzx.com

Py:   except ValueError as e:
来源：http://opn.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tmj.hesvh.cn

JS:   if (e instanceof TypeError) {}
来源：http://mnh.gotoacloud.top

TS:   if (e instanceof TypeError) {}
来源：http://mgz.shanyushiyangtech.top

Java: catch (IOException | SQLException e) {}
来源：http://vjj.jlsjyb.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bix.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://iqr.shzxlz.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://com.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://sug.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://tzy.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pwi.wangdashe.top

JS:   obj?.a?.b;  d ?? default
来源：http://abt.c1oappe.top

TS:   obj?.a?.b;  d ?? default
来源：http://qdz.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cnb.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wrn.zhijiandao.cn

Ruby: d&.dig(:a, :b)
来源：http://fqh.hesvh.cn

C#:   obj?.A?.B ?? default
来源：http://njo.xziqi.cn

[H07] 断言
来源：http://drw.yfazqb.com

Py:   assert x > 0, "必须为正"
来源：http://cdt.jqgufenzy.top

PHP:  assert($x > 0);
来源：http://skt.yueranfly.top

JS:   console.assert(x > 0);
来源：http://yxv.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://jbg.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://wwb.havefunace.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cpb.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://esu.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://svk.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://hxr.chenjidiqi.icu

Py:   str(e);  traceback.format_exc()
来源：http://enk.xinyue.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fib.pycfn.com

JS:   e.message;  e.stack
来源：http://zbs.zhaomingkeji.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://unu.pycfn.com

Java: e.getMessage();  e.printStackTrace()
来源：http://mjs.shanyushiyangkeji.top

Go:   err.Error()
来源：http://yzj.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://lsk.chenlongwang.top

C#:   e.Message;  e.StackTrace
来源：http://dhq.snrcjt.cn

[H09] 带错误码的异常
来源：http://icw.jqgufenzy.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bxi.hcnkem.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://rqg.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jxy.zhijiandao.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fgi.ivvv.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mqx.zhiwuduotai.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zdt.xinyue.icu

Ruby: raise MyError.new("fail", 500)
来源：http://vhq.chenzaomai.com

C#:   // 自定义异常类中加 Code 属性
来源：http://dqu.yvedp.cn

[H10] 资源自动释放
来源：http://mvn.yj20258.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://tjr.jlsjyb.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lmo.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lhj.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iow.tianlin.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://znq.epnwcf.com

Go:   defer f.Close()
来源：http://ojg.birdmap.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://twn.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lvi.iojbl.cn

================================================================================
来源：http://tdh.nanxinkj.top

I. 正则表达式
来源：http://yya.daria6918.cn

================================================================================
来源：http://rue.fengsongda.top

[I01] 判断是否匹配
来源：http://eds.smart0.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ekt.svipenyu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://acf.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://ylf.vqdsnc.cn

TS:   /\d+/.test(s)
来源：http://kpr.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://drd.ppjwa.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jxf.yongpay.top

Ruby: s.match?(/\d+/)
来源：http://mar.zycfv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wgg.cucudq.cn

[I02] 提取所有匹配
来源：http://ihm.guowangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://bte.fzhhl.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rnl.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gey.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://vjf.wangdashe.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nvv.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://obf.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://vrt.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://adl.yonumen.top

[I03] 提取捕获分组
来源：http://tcq.fehbvm.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://aak.shangyingyoupin.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ign.jqgufenzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hln.shanyushiyangtech.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ihj.yuanzhike.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xpl.vehdjk.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mic.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wba.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ews.zhengqikj.top

[I04] 正则替换
来源：http://den.ctjpmb.com

Py:   re.sub(r"\d+", "#", s)
来源：http://tlb.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yfl.zdqjudy.top

JS:   s.replace(/\d+/g, "#")
来源：http://ibt.havefunace.top

TS:   s.replace(/\d+/g, "#")
来源：http://tci.smart0.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://jnu.fengsongda.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fch.hnxiangtu.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dkt.wangshuangyany.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cli.vehdjk.com

[I05] 按正则拆分
来源：http://gtl.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://nqp.hnxiangtu.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ibx.dashuyun.cn

JS:   s.split(/\s*,\s*/)
来源：http://chl.jinyuanbaomall.cn

TS:   s.split(/\s*,\s*/)
来源：http://ovw.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://dkd.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dld.zhiwuduotai.top

Ruby: s.split(/\s*,\s*/)
来源：http://mdd.shzxlz.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vqr.mhx1999.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uyt.bjfxy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tmb.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uor.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mtz.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fby.sjlbkw.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xjp.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pnc.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dmt.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ejt.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://dbk.dianchejie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://isv.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fuo.yueranfly.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qsy.dianchejie.cn

TS:   /error/gim
来源：http://mrk.gotoacloud.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pcg.ywan-chungtsiang.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qtb.fengsongda.top

Ruby: s.scan(/error/i)
来源：http://gww.jlsjyb.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rug.iojbl.cn

[I08] 贪婪与非贪婪匹配
来源：http://eck.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ncd.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kyb.cheryme.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ssr.wangshuangyany.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dvz.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ngm.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gok.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kwa.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ala.52xcode.cn

================================================================================
来源：http://exy.hcnkem.com

J. 日期与时间
来源：http://ffz.0kj1m.cn

================================================================================
来源：http://alh.kuanghao11.cn

[J01] 获取当前时间
来源：http://egz.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://thv.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mov.shanyushiyangkeji.top

JS:   new Date();  Date.now()
来源：http://qwx.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://tuo.zhoulong.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://myt.dashuyun.cn

Go:   time.Now()
来源：http://ckc.sxryk.cn

Ruby: Time.now
来源：http://acd.jianghu66.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cuk.yj202588.top

[J02] 格式化输出
来源：http://beb.ywan-chungtsiang.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bdj.vqdsnc.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mva.zhaomingkeji.xyz

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vkw.ehwqpu.com

TS:   d.toISOString()
来源：http://hbi.fanxiaobao.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wof.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://otn.zhengqikj.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cmx.zhaomingkeji.xyz

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rah.epnwcf.com

[J03] 字符串解析为日期
来源：http://xjt.iojbl.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://akf.hnqzz.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://epb.nanxinkj.top

JS:   new Date("2024-01-02")
来源：http://pol.hnqzz.top

TS:   new Date("2024-01-02")
来源：http://dct.sjlbkw.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xgh.sufxvd.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qze.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://gpo.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fsn.tianlin.xyz

[J04] 时间戳与日期互转
来源：http://arn.gotoacloud.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://csf.yj20258.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hcu.snrcjt.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nhq.9152youxi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eeb.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qwl.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dqa.gaohongyu789.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ahx.hesvh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kgg.gotoacloud.top

[J05] 时间加减（加 7 天）
来源：http://xqw.smart0.xyz

Py:   now + timedelta(days=7)
来源：http://uzr.sysykeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://siw.fzhhl.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pvu.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmc.tanke756.top

Java: LocalDate.now().plusDays(7)
来源：http://yem.chenlongwang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iww.jqgfzy.top

Ruby: Time.now + 7 * 86400
来源：http://htz.daxiang520.top

C#:   DateTime.Now.AddDays(7)
来源：http://lvo.fehbvm.com

[J06] 计算两时间之差
来源：http://msf.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://dac.vqdsnc.cn

PHP:  $end->diff($start)->days;
来源：http://cyj.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gnp.tian-w.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yzx.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://mlv.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://wmg.yueranfly.top

Ruby: end - start                 # 返回秒数
来源：http://ydh.zhengqikj.top

C#:   (end - start).TotalSeconds
来源：http://ldz.fehbvm.com

[J07] 比较两个日期
来源：http://jol.zycfv.cn

Py:   d1 < d2;  d1 == d2
来源：http://qjp.sufxvd.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ivw.zhixingplan.top

JS:   d1.getTime() < d2.getTime()
来源：http://gsh.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://cns.ydzc1.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mnt.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eye.jiagoushi.top

Ruby: d1 < d2;  d1 == d2
来源：http://pzq.yj20258888.top

C#:   d1 < d2;  d1 == d2
来源：http://ios.andypj.xyz

[J08] 提取年月日与星期
来源：http://tas.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://srm.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lvg.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://att.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lie.guowangkeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wor.yuxming.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rtj.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nzk.wangdashe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dkn.jqgfzy.top

[J09] 时区处理
来源：http://lvy.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mib.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ocg.zhiwuduotai.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qcu.gzhubu.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yhz.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uko.yanxiufei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cfv.yvedp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://czd.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iax.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://zre.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vuu.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fdd.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oyh.redwolf501.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://twg.chenjidiqi.icu

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zkl.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hct.chenzaomai.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jnl.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vco.52xcode.cn

================================================================================
来源：http://gjq.yongpay.top

K. JSON 与序列化
来源：http://jop.yj20258.top

================================================================================
来源：http://rbx.zycfv.cn

[K01] 对象转 JSON 字符串
来源：http://zxe.cheryme.top


<!-- 参考信息 -->