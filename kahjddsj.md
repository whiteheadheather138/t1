代发 wailian999

Java: u instanceof User
来源：http://naj.ydzc1.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gjn.aizwys.cn

Ruby: u.is_a?(User)
来源：http://cyy.yj20258.top

C#:   u is User
来源：http://rxe.uphjek.com

[G14] 数据类 / record
来源：http://pea.snrcjt.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://omi.guowangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://wfp.iojbl.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wor.jiagoushi.top

TS:   type User = { name: string; age: number };
来源：http://nqo.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://qev.zhijiandao.cn

Go:   type User struct { Name string; Age int }
来源：http://efo.xuetiantiany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fxi.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://sdm.chenjidiqi.icu

[G15] 枚举
来源：http://pvo.0kj1m.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cqj.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://crm.cqqwz.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ubw.xuetiantiany.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ipz.hammf.cn

Java: enum Color { RED, GREEN }
来源：http://wxw.uphjek.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://njy.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://jvg.ctjpmb.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://plb.dashuyun.cn

[G16] 对象转数组 / 字典
来源：http://kmv.9152youxi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fsg.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://hft.xuanzx.com

JS:   Object.entries(obj)
来源：http://woo.dashuyun.cn

TS:   Object.entries(obj)
来源：http://toi.52xcode.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://faa.haohaochexian.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://cck.cheryme.top

Ruby: obj.instance_variables
来源：http://csr.jinqigufen.top

C#:   // 用反射或 System.Text.Json
来源：http://xrb.jinqigufen.top

================================================================================
来源：http://nvw.shanyushiyangkeji.top

H. 异常与错误处理
来源：http://lkc.yfazqb.com

================================================================================
来源：http://ajl.havefunace.top

[H01] try / catch 基础
来源：http://kqv.hnqzz.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rgm.zhiwuduotai.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xvc.sufxvd.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dkh.wangshuangyany.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jvy.zhaomingkeji.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jhc.jinyuanbaomall.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dmm.hfpthk.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ano.yfazqb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://klp.c1oappe.top

[H02] finally / ensure 收尾
来源：http://hho.yongpay.top

Py:   try: f()⏎finally: cleanup()
来源：http://xnd.yueranfly.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://rss.tanke756.top

JS:   try { f(); } finally { cleanup(); }
来源：http://asl.pycfn.com

TS:   try { f(); } finally { cleanup(); }
来源：http://ypq.hongshengwenyu.top

Java: try { f(); } finally { cleanup(); }
来源：http://whx.cheryme.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bxd.vehdjk.com

Ruby: begin; f; ensure; cleanup; end
来源：http://wcl.ivvv.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ony.yj20258888.top

[H03] 主动抛出异常
来源：http://gri.feifeiyinyue.top

Py:   raise ValueError("错误信息")
来源：http://sim.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dew.gotoacloud.top

JS:   throw new Error("错误信息");
来源：http://kmz.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://iwu.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ula.tanke756.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ybc.fzhhl.top

Ruby: raise ArgumentError, "错误信息"
来源：http://gta.ppjwa.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xjh.ctjpmb.com

[H04] 自定义异常类型
来源：http://dfp.jinghuilouyu.cn

Py:   class MyError(Exception): pass
来源：http://suo.52xcode.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fur.shuidangran.top

JS:   class MyError extends Error {}
来源：http://wfq.feifeiyinyue.top

TS:   class MyError extends Error {}
来源：http://hne.yangfankeji.com

Java: class MyException extends RuntimeException {}
来源：http://vhl.xylfe.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vad.dianchejie.cn

Ruby: class MyError < StandardError; end
来源：http://ffw.jyoumei.cn

C#:   class MyException : Exception {}
来源：http://bhb.fktsv.cn

[H05] 捕获特定类型
来源：http://uiy.jianghu66.top

Py:   except ValueError as e:
来源：http://pvi.gzhubu.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jei.hcnkem.com

JS:   if (e instanceof TypeError) {}
来源：http://ptc.hesvh.cn

TS:   if (e instanceof TypeError) {}
来源：http://xbv.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://pir.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fzw.yj20258888.top

Ruby: rescue ArgumentError => e
来源：http://pob.aizwys.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vqy.jyoumei.cn

[H06] 可选值 / 空值安全访问
来源：http://ewe.daxiang520.top

Py:   value = d.get("k") or default
来源：http://jpx.iojbl.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tgj.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nve.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fuy.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zux.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qge.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://yal.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://jfg.dianchejie.cn

[H07] 断言
来源：http://qri.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://ten.cheryme.top

PHP:  assert($x > 0);
来源：http://lik.quarkkingdee.top

JS:   console.assert(x > 0);
来源：http://yez.sxryk.cn

TS:   console.assert(x > 0);
来源：http://vir.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://cmi.pengpengdd.cyou

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tit.zhiwuduotai.top

Ruby: raise "必须为正" unless x > 0
来源：http://hqj.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://awt.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://wla.cucudq.cn

Py:   str(e);  traceback.format_exc()
来源：http://sys.ydjk.org.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hdv.aizwys.cn

JS:   e.message;  e.stack
来源：http://kuo.hnxiangtu.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xxr.shanyushiyangtech.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rol.xuetiantiany.cn

Go:   err.Error()
来源：http://pwk.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://alw.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://fcg.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://laf.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://evv.meibo888.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://hhe.shuidangran.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xfm.fanxiaobao.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ahi.cqqwz.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jdj.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wus.zhiwuduotai.top

Ruby: raise MyError.new("fail", 500)
来源：http://ffz.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://ytp.shanyushiyangtech.top

[H10] 资源自动释放
来源：http://pmh.zdbjq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ntq.gaohongyu789.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://phq.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qzm.hongshengwenyu.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dfw.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uwe.316326.xyz

Go:   defer f.Close()
来源：http://ppd.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mre.shzxlz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dkr.zhengqikj.top

================================================================================
来源：http://pru.mhx1999.top

I. 正则表达式
来源：http://jmx.havefunace.top

================================================================================
来源：http://mwb.snrcjt.cn

[I01] 判断是否匹配
来源：http://pwc.zdbjq.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dak.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ncm.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://pew.hammf.cn

TS:   /\d+/.test(s)
来源：http://mss.shanyushiyangtech.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vtn.fehbvm.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jup.jqgfzy.top

Ruby: s.match?(/\d+/)
来源：http://zst.hnqzz.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uqg.epnwcf.com

[I02] 提取所有匹配
来源：http://hum.aizwys.cn

Py:   re.findall(r"\d+", s)
来源：http://mud.yueranfly.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aan.svipenyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ghh.havefunace.top

TS:   s.match(/\d+/g)
来源：http://mar.chenlongwang.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yqn.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rct.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://aim.vehdjk.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tdr.yangfankeji.com

[I03] 提取捕获分组
来源：http://euq.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jzg.gaohongyu789.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wzt.iojbl.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zyl.epnwcf.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://btr.fzhhl.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ono.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jes.shanyushiyangtech.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vpu.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kqh.hcnkem.com

[I04] 正则替换
来源：http://fhk.xuetiantiany.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cjp.yuxming.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://der.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dkl.andypj.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://fjc.ydzc1.top

Java: s.replaceAll("\\d+", "#")
来源：http://tbd.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uly.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://cnz.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cbi.xylfe.cn

[I05] 按正则拆分
来源：http://nqw.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tsr.dianchejie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lso.jyoumei.cn

JS:   s.split(/\s*,\s*/)
来源：http://pjh.gzhubu.top

TS:   s.split(/\s*,\s*/)
来源：http://oem.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://msz.jinqigufen.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jrj.nanxinkj.top

Ruby: s.split(/\s*,\s*/)
来源：http://req.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sxs.fengsongda.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ugb.316326.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bkf.jianghu66.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jim.cucudq.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lzp.meibo888.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ozl.cheryme.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nlj.xylfe.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dtt.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xef.hysaishi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tzi.xziqi.cn

[I07] 忽略大小写与多行模式
来源：http://jts.yvedp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tyj.52xcode.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://spo.nanxuanxn.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bju.mhx1999.top

TS:   /error/gim
来源：http://uir.hnxiangtu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tox.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tke.bjfxy.top

Ruby: s.scan(/error/i)
来源：http://pam.aibaodan.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rgx.sjlbkw.cn

[I08] 贪婪与非贪婪匹配
来源：http://gyx.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lkt.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hiy.tianlin.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yhx.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mgj.hongshengwenyu.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://trh.xziqi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dau.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zmg.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://emw.jinqigfzy.top

================================================================================
来源：http://jfh.cdnleiting.top

J. 日期与时间
来源：http://ufc.daxiang520.top

================================================================================
来源：http://sby.gzhubu.top

[J01] 获取当前时间
来源：http://tsf.xylfe.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hjs.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://abx.jianghu66.top

JS:   new Date();  Date.now()
来源：http://xqb.fktsv.cn

TS:   new Date();  Date.now()
来源：http://cpo.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://urg.316326.xyz

Go:   time.Now()
来源：http://lhp.sysykeji.top

Ruby: Time.now
来源：http://rqt.guannengcc.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cqv.cheryme.top

[J02] 格式化输出
来源：http://aqi.cqqwz.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dey.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hvy.ppjwa.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mtq.tanke756.top

TS:   d.toISOString()
来源：http://oic.yonumen.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tfp.zhiwuduotai.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gdj.dianchejie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wen.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yha.haohaochexian.top

[J03] 字符串解析为日期
来源：http://heu.yj20258.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pmv.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zkc.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://xxo.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://jls.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hnx.gzhubu.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gmb.zhiwuduotai.top

Ruby: Date.parse("2024-01-02")
来源：http://ftg.birdmap.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lab.zhongyouzk.top

[J04] 时间戳与日期互转
来源：http://soo.jqgufenzy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lps.xuanzx.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ltw.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jvg.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://zla.hysaishi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hwv.dianchejie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://msz.meibo888.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cfk.ppjwa.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ydx.fehbvm.com

[J05] 时间加减（加 7 天）
来源：http://ehf.dianchejie.cn

Py:   now + timedelta(days=7)
来源：http://idd.wangshuangyany.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://bkt.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kmg.fzhhl.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hsq.shanyushiyangkeji.top

Java: LocalDate.now().plusDays(7)
来源：http://gsg.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mjc.jinghuilouyu.cn

Ruby: Time.now + 7 * 86400
来源：http://omw.yj20258888.top

C#:   DateTime.Now.AddDays(7)
来源：http://agt.ivvv.top

[J06] 计算两时间之差
来源：http://bid.chenjidiqi.icu

Py:   (end - start).total_seconds()
来源：http://svw.daxiang520.top

PHP:  $end->diff($start)->days;
来源：http://llb.fzhhl.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://woj.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ase.jqgfzy.top

Java: Duration.between(start, end).toSeconds()
来源：http://wsp.hfpthk.cn

Go:   end.Sub(start).Hours()
来源：http://xvr.kuanghao11.cn

Ruby: end - start                 # 返回秒数
来源：http://fav.cheryme.top

C#:   (end - start).TotalSeconds
来源：http://hqd.hfpthk.cn

[J07] 比较两个日期
来源：http://vwj.birdmap.top

Py:   d1 < d2;  d1 == d2
来源：http://szh.feifeiyinyue.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xrf.fzhhl.top

JS:   d1.getTime() < d2.getTime()
来源：http://atv.shuidangran.top

TS:   d1.getTime() < d2.getTime()
来源：http://tvo.gogol.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dcq.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nas.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tpt.sjlbkw.cn

C#:   d1 < d2;  d1 == d2
来源：http://dhu.birdmap.top

[J08] 提取年月日与星期
来源：http://wkd.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kjn.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eqv.redwolf501.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sdd.yj20258.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qww.vqdsnc.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://and.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bpu.ehwqpu.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wkf.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bpk.yangfankeji.com

[J09] 时区处理
来源：http://xjm.yj20258.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dpc.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tyb.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ekk.daria6918.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abj.dianchejie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gnu.yuanzhike.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tps.bbcook.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ezd.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rss.gzhubu.top

[J10] 取今天 / 本月第一天
来源：http://ycg.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://eyo.dianchejie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://odw.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dcv.dianchejie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jig.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gmb.hysaishi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rkp.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zrp.pycfn.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mfm.shuidangran.top

================================================================================
来源：http://hpd.zhaomingkeji.xyz

K. JSON 与序列化
来源：http://utw.gzhubu.top

================================================================================
来源：http://acf.chenjidiqi.icu

[K01] 对象转 JSON 字符串
来源：http://awz.fktsv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bdf.dianchejie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fjq.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://hsa.zhiwuduotai.top

TS:   JSON.stringify(obj)
来源：http://alo.sxryk.cn


<!-- 参考信息 -->