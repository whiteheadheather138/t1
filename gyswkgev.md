代发 wailian999

[G14] 数据类 / record
来源：http://qeb.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hsu.tianlin.xyz

PHP:  // 用 readonly 属性模拟
来源：http://gqc.aibaodan.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uiw.guannengcc.top

TS:   type User = { name: string; age: number };
来源：http://itu.fzhhl.top

Java: record User(String name, int age) {}
来源：http://dkl.shuidangran.top

Go:   type User struct { Name string; Age int }
来源：http://omr.jiagoushi.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ari.yfazqb.com

C#:   record User(string Name, int Age);
来源：http://ecs.ehwqpu.com

[G15] 枚举
来源：http://mpp.shanyushiyangtech.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://flo.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://pjj.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://aew.birdmap.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oqo.fktsv.cn

Java: enum Color { RED, GREEN }
来源：http://lie.fanxiaobao.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ylw.zdqjudy.top

Ruby: Color = %i[red green].freeze
来源：http://age.andypj.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hvh.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://xjk.sjlbkw.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://msi.cashguo.top

PHP:  get_object_vars($obj);
来源：http://mus.ydjk.org.cn

JS:   Object.entries(obj)
来源：http://mgz.yj20258888.top

TS:   Object.entries(obj)
来源：http://dpd.sufxvd.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bni.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://eli.quarkkingdee.top

Ruby: obj.instance_variables
来源：http://dnc.nwbrower.top

C#:   // 用反射或 System.Text.Json
来源：http://usz.hesvh.cn

================================================================================
来源：http://gal.cheryme.top

H. 异常与错误处理
来源：http://qxq.shanyushiyangkeji.top

================================================================================
来源：http://wmp.dianchejie.cn

[H01] try / catch 基础
来源：http://rik.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://msp.ppjwa.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qbb.zhiwuduotai.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cze.ehwqpu.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mfr.sufxvd.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mon.meibo888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lst.chenlongwang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ira.epnwcf.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ldh.xuetiantiany.cn

[H02] finally / ensure 收尾
来源：http://zsc.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://tcq.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://eeo.daxiang520.top

JS:   try { f(); } finally { cleanup(); }
来源：http://dsw.chenzaomai.com

TS:   try { f(); } finally { cleanup(); }
来源：http://vxy.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://oyw.haohaochexian.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rcy.bjfxy.top

Ruby: begin; f; ensure; cleanup; end
来源：http://eig.guannengcc.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ulc.zhixingplan.top

[H03] 主动抛出异常
来源：http://pyt.hesvh.cn

Py:   raise ValueError("错误信息")
来源：http://wkb.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hqz.cheryme.top

JS:   throw new Error("错误信息");
来源：http://ezd.ybcxt.top

TS:   throw new Error("错误信息");
来源：http://mlb.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lyy.sjlbkw.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rhe.hnxiangtu.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sqb.316326.xyz

C#:   throw new ArgumentException("错误信息");
来源：http://scp.ivvv.top

[H04] 自定义异常类型
来源：http://raf.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://hxz.zhoulong.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://fqs.bbcook.cn

JS:   class MyError extends Error {}
来源：http://ept.hnqzz.top

TS:   class MyError extends Error {}
来源：http://ajh.gogol.net.cn

Java: class MyException extends RuntimeException {}
来源：http://nhl.yj20258888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ivi.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://nlc.jinqigfzy.top

C#:   class MyException : Exception {}
来源：http://ibj.smart0.xyz

[H05] 捕获特定类型
来源：http://vre.gzhubu.top

Py:   except ValueError as e:
来源：http://snh.meibo888.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bzp.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://zgu.quarkkingdee.top

TS:   if (e instanceof TypeError) {}
来源：http://awr.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://kmh.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cwy.fengsongda.top

Ruby: rescue ArgumentError => e
来源：http://bew.yvedp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xrp.xinyue.icu

[H06] 可选值 / 空值安全访问
来源：http://ckm.fanxiaobao.xyz

Py:   value = d.get("k") or default
来源：http://mvx.c1oappe.top

PHP:  $v = $d["k"] ?? null;
来源：http://jur.pengpengdd.cyou

JS:   obj?.a?.b;  d ?? default
来源：http://dcs.ivvv.top

TS:   obj?.a?.b;  d ?? default
来源：http://pxz.0kj1m.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ese.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vxt.bbcook.cn

Ruby: d&.dig(:a, :b)
来源：http://adq.epnwcf.com

C#:   obj?.A?.B ?? default
来源：http://jmc.hammf.cn

[H07] 断言
来源：http://imd.ctjpmb.com

Py:   assert x > 0, "必须为正"
来源：http://dge.ppjwa.cn

PHP:  assert($x > 0);
来源：http://sal.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://lsd.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://cgv.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://kgy.c1oappe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jhu.zhijiandao.cn

Ruby: raise "必须为正" unless x > 0
来源：http://emf.jianghu66.top

C#:   Debug.Assert(x > 0);
来源：http://zdf.jqgfzy.top

[H08] 获取错误信息与堆栈
来源：http://rvd.vehdjk.com

Py:   str(e);  traceback.format_exc()
来源：http://hlg.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dem.birdmap.top

JS:   e.message;  e.stack
来源：http://zvz.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cfh.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ygs.tanke756.top

Go:   err.Error()
来源：http://tcu.sjlbkw.cn

Ruby: e.message;  e.backtrace
来源：http://bou.yfazqb.com

C#:   e.Message;  e.StackTrace
来源：http://sgd.andypj.xyz

[H09] 带错误码的异常
来源：http://hos.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mci.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tjd.sweek.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rfd.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fdb.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nqx.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qmc.guowangkeji.top

Ruby: raise MyError.new("fail", 500)
来源：http://vtt.zhixingplan.top

C#:   // 自定义异常类中加 Code 属性
来源：http://dbi.cashguo.top

[H10] 资源自动释放
来源：http://kon.yfazqb.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://pxq.ppjwa.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nzd.uphjek.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iyp.hfpthk.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eri.yj202588.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://suw.wangshuangyany.cn

Go:   defer f.Close()
来源：http://jsu.fengsongda.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wwh.feifeiyinyue.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wdb.bjfxy.top

================================================================================
来源：http://qew.gogol.net.cn

I. 正则表达式
来源：http://czc.zdqjudy.top

================================================================================
来源：http://fgp.redwolf501.top

[I01] 判断是否匹配
来源：http://xpp.ehwqpu.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aru.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://nfb.shanyushiyangkeji.top

JS:   /\d+/.test(s)
来源：http://din.chenlongwang.top

TS:   /\d+/.test(s)
来源：http://jev.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nch.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gms.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://jle.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gov.tian-w.cn

[I02] 提取所有匹配
来源：http://bjp.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://qlo.shanyushiyangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cum.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ezg.9152youxi.cn

TS:   s.match(/\d+/g)
来源：http://mav.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tty.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ssn.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://dmw.gzhubu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ztv.fanxiaobao.xyz

[I03] 提取捕获分组
来源：http://ksw.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://haf.jiagoushi.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qdm.jinqigufen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qcj.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mcq.wangdashe.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eop.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fbk.chenzaomai.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dwk.svipenyu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://efg.redwolf501.top

[I04] 正则替换
来源：http://dqw.sxryk.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://piq.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uzs.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://fch.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kiz.yangfankeji.com

Java: s.replaceAll("\\d+", "#")
来源：http://sed.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://usr.zdqjudy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hrq.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lki.zhongyouzk.top

[I05] 按正则拆分
来源：http://stw.mhx1999.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bbr.hfpthk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mhq.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://atc.fehbvm.com

TS:   s.split(/\s*,\s*/)
来源：http://syu.ydjk.org.cn

Java: s.split("\\s*,\\s*")
来源：http://lpb.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uhe.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ekc.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://efs.sjlbkw.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yfz.ydjk.org.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sdo.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kae.0kj1m.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nxd.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zna.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xvh.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vzq.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lan.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://aqr.jinqigfzy.top

[I07] 忽略大小写与多行模式
来源：http://nyx.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ewj.fzhhl.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gki.fktsv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rbb.yj202588.top

TS:   /error/gim
来源：http://ooq.ctjpmb.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vmi.dashuyun.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vxi.yj202588.top

Ruby: s.scan(/error/i)
来源：http://lhi.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ond.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://tnk.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mqm.daria6918.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://aad.sjlbkw.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kou.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yuw.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tfk.iojbl.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ipu.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dvr.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cty.zhoulong.xyz

================================================================================
来源：http://gvd.hnxiangtu.top

J. 日期与时间
来源：http://pts.hysaishi.cn

================================================================================
来源：http://dvs.yuxming.cn

[J01] 获取当前时间
来源：http://ycq.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eit.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zpt.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://arv.wangshuangyany.cn

TS:   new Date();  Date.now()
来源：http://laq.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://rhc.zhiwuduotai.top

Go:   time.Now()
来源：http://suj.haohaochexian.top

Ruby: Time.now
来源：http://byq.dashuyun.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xyj.hnxiangtu.top

[J02] 格式化输出
来源：http://dkr.jinqigufen.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yfd.hongshengwenyu.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dxq.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://eua.shanyushiyangkeji.top

TS:   d.toISOString()
来源：http://ujb.pycfn.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://emr.xingfuxueyuan.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvw.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cwq.shuidangran.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ygc.yj202588.top

[J03] 字符串解析为日期
来源：http://pdi.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://uuz.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nls.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://htv.9152youxi.cn

TS:   new Date("2024-01-02")
来源：http://mrq.fehbvm.com

Java: LocalDate.parse("2024-01-02")
来源：http://rlo.xuanzx.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hvb.gzhubu.top

Ruby: Date.parse("2024-01-02")
来源：http://hjp.tianlin.xyz

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dzq.hesvh.cn

[J04] 时间戳与日期互转
来源：http://dsw.jinghuilouyu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xvo.daxiang520.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://moh.zhijiandao.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://obx.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jgw.chenjidiqi.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vec.uphjek.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ybq.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rmj.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vdx.smart0.xyz

[J05] 时间加减（加 7 天）
来源：http://ndd.daxiang520.top

Py:   now + timedelta(days=7)
来源：http://ylv.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tho.uphjek.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bpf.zycfv.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fuc.daxiang520.top

Java: LocalDate.now().plusDays(7)
来源：http://wal.pengpengdd.cyou

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gtl.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://fym.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://ghe.aizwys.cn

[J06] 计算两时间之差
来源：http://jxk.meibo888.top

Py:   (end - start).total_seconds()
来源：http://eqt.dianchejie.cn

PHP:  $end->diff($start)->days;
来源：http://dzo.chenjidiqi.icu

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pji.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aet.zhengqikj.top

Java: Duration.between(start, end).toSeconds()
来源：http://iil.jlsjyb.cn

Go:   end.Sub(start).Hours()
来源：http://jaa.yfazqb.com

Ruby: end - start                 # 返回秒数
来源：http://myd.cucudq.cn

C#:   (end - start).TotalSeconds
来源：http://cjt.316326.xyz

[J07] 比较两个日期
来源：http://jol.gogol.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://bcx.shuidangran.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jgq.jqgufenzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://beo.zdbjq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://iol.ydjk.org.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tic.zdqjudy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lem.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://cof.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://axz.havefunace.top

[J08] 提取年月日与星期
来源：http://slo.ywan-chungtsiang.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jne.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://win.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://khv.xuanzx.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ftu.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uvn.yanxiufei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wjs.zhoulong.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lnc.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pus.zhixingplan.top

[J09] 时区处理
来源：http://zat.snrcjt.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lja.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yso.xinyue.icu

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vag.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hym.yj202588.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://flb.zhaomingkeji.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jge.redwolf501.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kuo.hammf.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://orq.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://qju.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vef.xuanzx.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mmc.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pku.cqqwz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fii.yangfankeji.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://byl.zhongyouzk.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrj.sysykeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mgp.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nhc.yanxiufei.cn

================================================================================
来源：http://bkw.fehbvm.com

K. JSON 与序列化
来源：http://tgh.ivvv.top

================================================================================
来源：http://iqg.yvedp.cn

[K01] 对象转 JSON 字符串
来源：http://yyf.uphjek.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rsw.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jmd.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://irp.ivvv.top

TS:   JSON.stringify(obj)
来源：http://ejo.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bgq.tian-w.cn

Go:   json.Marshal(obj)
来源：http://gcu.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://upn.epnwcf.com

C#:   JsonSerializer.Serialize(obj)
来源：http://chn.yj20258.top


<!-- 参考信息 -->