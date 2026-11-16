代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://fcv.cheryme.top

Java: record User(String name, int age) {}
来源：http://eks.zhengqikj.top

Go:   type User struct { Name string; Age int }
来源：http://fvs.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://czm.cashguo.top

C#:   record User(string Name, int Age);
来源：http://wfx.sjlbkw.cn

[G15] 枚举
来源：http://jap.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oqx.epnwcf.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://bsr.jinqigfzy.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rts.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kfj.yuxming.cn

Java: enum Color { RED, GREEN }
来源：http://nlc.ehwqpu.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://agk.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://svf.cdnleiting.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fxq.hysaishi.cn

[G16] 对象转数组 / 字典
来源：http://nei.cqqwz.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xsn.cheryme.top

PHP:  get_object_vars($obj);
来源：http://mgr.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://ptz.yueranfly.top

TS:   Object.entries(obj)
来源：http://rke.sweek.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://myk.kuanghao11.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aja.haohaochexian.top

Ruby: obj.instance_variables
来源：http://rfv.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://onz.meibo888.top

================================================================================
来源：http://fxx.shanyushiyangtech.top

H. 异常与错误处理
来源：http://idp.jinqigufen.top

================================================================================
来源：http://sdx.yanxiufei.cn

[H01] try / catch 基础
来源：http://get.zhiwuduotai.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mjz.tarul.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dhd.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aei.gzhubu.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ngm.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wbi.shzxlz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://crk.jinqigufen.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xmk.daxiang520.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ryg.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://wpq.sjlbkw.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ong.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zzo.jiagoushi.top

JS:   try { f(); } finally { cleanup(); }
来源：http://mty.jiagoushi.top

TS:   try { f(); } finally { cleanup(); }
来源：http://hlm.havefunace.top

Java: try { f(); } finally { cleanup(); }
来源：http://fzn.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://rzd.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://hmb.gaohongyu789.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xij.sysykeji.top

[H03] 主动抛出异常
来源：http://cec.yanxiufei.cn

Py:   raise ValueError("错误信息")
来源：http://bae.yj20258.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dlo.fehbvm.com

JS:   throw new Error("错误信息");
来源：http://wqp.hywenlv.cn

TS:   throw new Error("错误信息");
来源：http://xen.sjlbkw.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hlv.pycfn.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xhn.shanyushiyangkeji.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pby.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://szv.fengsongda.top

[H04] 自定义异常类型
来源：http://hbk.uphjek.com

Py:   class MyError(Exception): pass
来源：http://ybx.mhx1999.top

PHP:  class MyError extends RuntimeException {}
来源：http://vac.bbcook.cn

JS:   class MyError extends Error {}
来源：http://saq.birdmap.top

TS:   class MyError extends Error {}
来源：http://qsy.shanyushiyangtech.top

Java: class MyException extends RuntimeException {}
来源：http://afr.nanxuanxn.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zwh.hysaishi.cn

Ruby: class MyError < StandardError; end
来源：http://hpp.hywenlv.cn

C#:   class MyException : Exception {}
来源：http://fem.ydzc1.top

[H05] 捕获特定类型
来源：http://wsy.andypj.xyz

Py:   except ValueError as e:
来源：http://ola.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nfy.tanke756.top

JS:   if (e instanceof TypeError) {}
来源：http://evy.haohaochexian.top

TS:   if (e instanceof TypeError) {}
来源：http://ebe.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://zyw.vehdjk.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hqe.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://byq.guowangkeji.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wws.tian-w.cn

[H06] 可选值 / 空值安全访问
来源：http://wqt.sxryk.cn

Py:   value = d.get("k") or default
来源：http://dce.tian-w.cn

PHP:  $v = $d["k"] ?? null;
来源：http://arq.pycfn.com

JS:   obj?.a?.b;  d ?? default
来源：http://alf.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://yvj.shzxlz.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vvw.jyoumei.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pkp.sufxvd.cn

Ruby: d&.dig(:a, :b)
来源：http://hph.yj20258888.top

C#:   obj?.A?.B ?? default
来源：http://jon.vqdsnc.cn

[H07] 断言
来源：http://dkt.hongshengwenyu.top

Py:   assert x > 0, "必须为正"
来源：http://ndj.iojbl.cn

PHP:  assert($x > 0);
来源：http://cpi.ybcxt.top

JS:   console.assert(x > 0);
来源：http://pyr.shangyingyoupin.top

TS:   console.assert(x > 0);
来源：http://xzh.yj202588.top

Java: assert x > 0 : "必须为正";
来源：http://qqu.tian-w.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kbr.ivvv.top

Ruby: raise "必须为正" unless x > 0
来源：http://nsh.ydjk.org.cn

C#:   Debug.Assert(x > 0);
来源：http://myg.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://xul.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://dvg.dashuyun.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bpe.guannengcc.top

JS:   e.message;  e.stack
来源：http://wsf.ivvv.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xoq.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hww.gzhubu.top

Go:   err.Error()
来源：http://pqs.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://xzz.pengpengdd.cyou

C#:   e.Message;  e.StackTrace
来源：http://rmi.hysaishi.cn

[H09] 带错误码的异常
来源：http://dyk.zhijiandao.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bvs.yanxiufei.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pjl.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lyu.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zvr.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sqd.vehdjk.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fvk.meibo888.top

Ruby: raise MyError.new("fail", 500)
来源：http://cnu.guannengcc.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bbu.jqgfzy.top

[H10] 资源自动释放
来源：http://bek.vqdsnc.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fpe.nwbrower.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wkk.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mte.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oar.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ior.vehdjk.com

Go:   defer f.Close()
来源：http://jir.nanxuanxn.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://que.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://stj.ydjk.org.cn

================================================================================
来源：http://zjf.snrcjt.cn

I. 正则表达式
来源：http://vww.9152youxi.cn

================================================================================
来源：http://hys.cheryme.top

[I01] 判断是否匹配
来源：http://sib.jinyuanbaomall.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kgv.ydzc1.top

PHP:  preg_match('/\d+/', $s);
来源：http://nnd.kuanghao11.cn

JS:   /\d+/.test(s)
来源：http://qgp.fehbvm.com

TS:   /\d+/.test(s)
来源：http://qiz.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fmf.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ebb.ctjpmb.com

Ruby: s.match?(/\d+/)
来源：http://axu.ybcxt.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yvf.haohaochexian.top

[I02] 提取所有匹配
来源：http://pjo.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://thu.xingfuxueyuan.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vgz.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wju.birdmap.top

TS:   s.match(/\d+/g)
来源：http://vzh.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hst.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ydg.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://ows.smart0.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ndm.kuanghao11.cn

[I03] 提取捕获分组
来源：http://qjl.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vct.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zkv.epnwcf.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ixm.vqdsnc.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tjm.52xcode.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nui.vqdsnc.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://erw.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qaf.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rge.yueranfly.top

[I04] 正则替换
来源：http://rar.fktsv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rrk.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mro.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hcy.yj20258.top

TS:   s.replace(/\d+/g, "#")
来源：http://ory.tianlin.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://qup.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://hqe.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ras.bbcook.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jsu.zhengqikj.top

[I05] 按正则拆分
来源：http://ryn.andypj.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://chy.sxryk.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mbo.zycfv.cn

JS:   s.split(/\s*,\s*/)
来源：http://jid.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://vgz.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://iry.smart0.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pnh.sysykeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://rqx.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uls.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ywf.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dzr.c1oappe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dzx.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://icd.nwbrower.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jfn.sysykeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cbi.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hds.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://meh.zhijiandao.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lxv.jyoumei.cn

[I07] 忽略大小写与多行模式
来源：http://gjy.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rxp.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dhv.yongpay.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wfx.cdnleiting.top

TS:   /error/gim
来源：http://phn.pycfn.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xuu.shanyushiyangtech.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://krq.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://cao.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rtz.smart0.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ywr.tanke756.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bdj.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nlm.jinqigufen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kkv.cqqwz.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xww.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bon.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qvz.shanyushiyangkeji.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zxi.guannengcc.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wnj.316326.xyz

================================================================================
来源：http://nlb.fzhhl.top

J. 日期与时间
来源：http://hil.52xcode.cn

================================================================================
来源：http://ggy.iojbl.cn

[J01] 获取当前时间
来源：http://ufb.andypj.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://lrw.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xmc.0kj1m.cn

JS:   new Date();  Date.now()
来源：http://lvr.aizwys.cn

TS:   new Date();  Date.now()
来源：http://pnp.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ebo.jqgufenzy.top

Go:   time.Now()
来源：http://ttf.shanyushiyangkeji.top

Ruby: Time.now
来源：http://zbm.aizwys.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pgw.epnwcf.com

[J02] 格式化输出
来源：http://rxw.ehwqpu.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hsw.tanke756.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wdj.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ino.tarul.cn

TS:   d.toISOString()
来源：http://ihr.guannengcc.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lqn.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jed.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxd.shanyushiyangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cie.aizwys.cn

[J03] 字符串解析为日期
来源：http://ptr.yangfankeji.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rqz.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nxu.zycfv.cn

JS:   new Date("2024-01-02")
来源：http://ccm.jinqigfzy.top

TS:   new Date("2024-01-02")
来源：http://shr.zhaomingkeji.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://qru.c1oappe.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hdq.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://lhv.gotoacloud.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://pit.aizwys.cn

[J04] 时间戳与日期互转
来源：http://aqc.yongpay.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://efx.epnwcf.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ous.shanyushiyangtech.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hph.gaohongyu789.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nni.xziqi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ctq.yuxming.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://acw.pycfn.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cai.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://swe.shuidangran.top

[J05] 时间加减（加 7 天）
来源：http://zwk.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://llj.aizwys.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xka.redwolf501.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://yzv.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kby.meibo888.top

Java: LocalDate.now().plusDays(7)
来源：http://gzj.ywan-chungtsiang.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vrb.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://ykd.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gmo.jqgfzy.top

[J06] 计算两时间之差
来源：http://yrg.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://mes.jinghuilouyu.cn

PHP:  $end->diff($start)->days;
来源：http://weg.ywan-chungtsiang.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gao.gogol.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://efm.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://emk.xuetiantiany.cn

Go:   end.Sub(start).Hours()
来源：http://gbs.zdqjudy.top

Ruby: end - start                 # 返回秒数
来源：http://eau.ybcxt.top

C#:   (end - start).TotalSeconds
来源：http://tqc.cucudq.cn

[J07] 比较两个日期
来源：http://tup.shangyingyoupin.top

Py:   d1 < d2;  d1 == d2
来源：http://dkz.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://thx.fanxiaobao.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://wkq.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://jfr.vqdsnc.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qqq.daxiang520.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ysw.jinghuilouyu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lie.cashguo.top

C#:   d1 < d2;  d1 == d2
来源：http://zgi.fehbvm.com

[J08] 提取年月日与星期
来源：http://vqq.hcnkem.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://voi.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zve.jqgfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dze.zhijiandao.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lpt.quarkkingdee.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kok.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lft.fktsv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xcx.hysaishi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vbi.aizwys.cn

[J09] 时区处理
来源：http://yfa.c1oappe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lqk.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cdu.sysykeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mea.cheryme.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mlt.tanke756.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yur.iojbl.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ari.fktsv.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lqk.redwolf501.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kgx.shanyushiyangtech.top

[J10] 取今天 / 本月第一天
来源：http://jtt.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://pms.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://him.andypj.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://cuo.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ifs.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ptm.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ewc.hcnkem.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lgu.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cyn.zhoulong.xyz

================================================================================
来源：http://mcm.snrcjt.cn

K. JSON 与序列化
来源：http://xnv.yj20258888.top

================================================================================
来源：http://ozt.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://qmn.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lsl.hongshengwenyu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pae.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://egw.yuanzhike.top

TS:   JSON.stringify(obj)
来源：http://gzd.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vhn.meibo888.top

Go:   json.Marshal(obj)
来源：http://ies.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://jbi.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ofw.ivvv.top

[K02] JSON 字符串转对象
来源：http://hsk.fktsv.cn

Py:   json.loads(s)
来源：http://kka.gaohongyu789.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xbp.haohaochexian.top

JS:   JSON.parse(s)
来源：http://otr.jianghu66.top


<!-- 参考信息 -->