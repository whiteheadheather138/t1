代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zsx.zycfv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uwo.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rbm.jqgufenzy.top

[H02] finally / ensure 收尾
来源：http://qng.meibo888.top

Py:   try: f()⏎finally: cleanup()
来源：http://gzs.chenzaomai.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://rej.tianlin.xyz

JS:   try { f(); } finally { cleanup(); }
来源：http://cxo.jianghu66.top

TS:   try { f(); } finally { cleanup(); }
来源：http://gnv.jyoumei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kpc.dianchejie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cmv.zhixingplan.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xwe.feifeiyinyue.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://hkg.snrcjt.cn

[H03] 主动抛出异常
来源：http://vsl.shanyushiyangkeji.top

Py:   raise ValueError("错误信息")
来源：http://das.gogol.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://eeo.tanke756.top

JS:   throw new Error("错误信息");
来源：http://olh.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://pql.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://san.smart0.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kpq.jinqigfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bjg.shangyingyoupin.top

C#:   throw new ArgumentException("错误信息");
来源：http://nlf.yuxming.cn

[H04] 自定义异常类型
来源：http://cea.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://xuh.fktsv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wzt.quarkkingdee.top

JS:   class MyError extends Error {}
来源：http://bvk.aizwys.cn

TS:   class MyError extends Error {}
来源：http://rmf.hysaishi.cn

Java: class MyException extends RuntimeException {}
来源：http://wdj.guannengcc.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://euu.zdqjudy.top

Ruby: class MyError < StandardError; end
来源：http://ajc.yuxming.cn

C#:   class MyException : Exception {}
来源：http://dik.iojbl.cn

[H05] 捕获特定类型
来源：http://dxq.yongpay.top

Py:   except ValueError as e:
来源：http://zur.9152youxi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bsz.jinqigfzy.top

JS:   if (e instanceof TypeError) {}
来源：http://bfu.9152youxi.cn

TS:   if (e instanceof TypeError) {}
来源：http://qvo.bbcook.cn

Java: catch (IOException | SQLException e) {}
来源：http://dbz.guowangkeji.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://swb.9152youxi.cn

Ruby: rescue ArgumentError => e
来源：http://ste.vehdjk.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hru.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://bmi.bbcook.cn

Py:   value = d.get("k") or default
来源：http://xzx.ywan-chungtsiang.top

PHP:  $v = $d["k"] ?? null;
来源：http://zwr.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vgp.xuetiantiany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fbj.yj20258888.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ytf.ppjwa.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://evp.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://mbo.jianghu66.top

C#:   obj?.A?.B ?? default
来源：http://eef.ivvv.top

[H07] 断言
来源：http://bpp.wangdashe.top

Py:   assert x > 0, "必须为正"
来源：http://shd.aizwys.cn

PHP:  assert($x > 0);
来源：http://mso.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://wzq.jqgfzy.top

TS:   console.assert(x > 0);
来源：http://boa.shanyushiyangtech.top

Java: assert x > 0 : "必须为正";
来源：http://oek.epnwcf.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uuf.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bfk.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://uzy.snrcjt.cn

[H08] 获取错误信息与堆栈
来源：http://lnj.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://rgm.vehdjk.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bvy.tianlin.xyz

JS:   e.message;  e.stack
来源：http://vmb.yj20258.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xya.hysaishi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bur.yvedp.cn

Go:   err.Error()
来源：http://orj.hesvh.cn

Ruby: e.message;  e.backtrace
来源：http://xoq.zdqjudy.top

C#:   e.Message;  e.StackTrace
来源：http://auc.yvedp.cn

[H09] 带错误码的异常
来源：http://tfu.hnqzz.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lhk.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://nrb.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bvk.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bvd.zhixingplan.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kvr.xinyue.icu

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vys.jinyuanbaomall.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nrp.guowangkeji.top

C#:   // 自定义异常类中加 Code 属性
来源：http://bih.fzhhl.top

[H10] 资源自动释放
来源：http://vnt.daxiang520.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://wvl.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://brz.zhixingplan.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gmj.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vlh.kuanghao11.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gpx.xziqi.cn

Go:   defer f.Close()
来源：http://qil.shzxlz.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://enw.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nev.jqgufenzy.top

================================================================================
来源：http://axs.andypj.xyz

I. 正则表达式
来源：http://mfi.daria6918.cn

================================================================================
来源：http://hjj.jqgfzy.top

[I01] 判断是否匹配
来源：http://wfi.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lwj.zhixingplan.top

PHP:  preg_match('/\d+/', $s);
来源：http://jip.tanke756.top

JS:   /\d+/.test(s)
来源：http://anr.fengsongda.top

TS:   /\d+/.test(s)
来源：http://pgv.dianchejie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bex.wangdashe.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vqe.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://gil.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vqh.aizwys.cn

[I02] 提取所有匹配
来源：http://rgj.cashguo.top

Py:   re.findall(r"\d+", s)
来源：http://epo.bbcook.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pqg.sweek.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://whg.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://aio.quarkkingdee.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wnm.ybcxt.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://our.hcnkem.com

Ruby: s.scan(/\d+/)
来源：http://szw.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://phx.birdmap.top

[I03] 提取捕获分组
来源：http://jrh.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dzz.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ysn.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gxg.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xrm.xingfuxueyuan.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ymi.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hgx.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fdn.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://apu.yuxming.cn

[I04] 正则替换
来源：http://ioe.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://jds.tanke756.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xki.tian-w.cn

JS:   s.replace(/\d+/g, "#")
来源：http://llb.sweek.top

TS:   s.replace(/\d+/g, "#")
来源：http://aha.pengpengdd.cyou

Java: s.replaceAll("\\d+", "#")
来源：http://wcv.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://sog.zhiwuduotai.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jwf.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pwt.havefunace.top

[I05] 按正则拆分
来源：http://mny.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://axl.ybcxt.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xhk.shanyushiyangtech.top

JS:   s.split(/\s*,\s*/)
来源：http://zhn.yfazqb.com

TS:   s.split(/\s*,\s*/)
来源：http://xeg.9152youxi.cn

Java: s.split("\\s*,\\s*")
来源：http://bmn.hcnkem.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gdo.316326.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://zos.yuxming.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jse.quarkkingdee.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jvf.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://chw.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://das.ivvv.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ddg.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wek.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tha.birdmap.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fhj.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qqt.fzhhl.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qbs.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://xct.bjfxy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aqa.hfpthk.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fra.yanxiufei.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rhx.zdbjq.cn

TS:   /error/gim
来源：http://yik.hcnkem.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uem.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://opb.ivvv.top

Ruby: s.scan(/error/i)
来源：http://tzl.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://swa.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://dfl.shuidangran.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gvp.jianghu66.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yzf.fengsongda.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sxm.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dai.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fwe.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ocb.cdnleiting.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vlz.haohaochexian.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nny.nanxinkj.top

================================================================================
来源：http://nrq.andypj.xyz

J. 日期与时间
来源：http://pjd.birdmap.top

================================================================================
来源：http://hah.fzhhl.top

[J01] 获取当前时间
来源：http://qgm.yj20258.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://hth.aizwys.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bsg.ydjk.org.cn

JS:   new Date();  Date.now()
来源：http://aff.cucudq.cn

TS:   new Date();  Date.now()
来源：http://rxz.tianlin.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://vjv.fengsongda.top

Go:   time.Now()
来源：http://ctj.ywan-chungtsiang.top

Ruby: Time.now
来源：http://foe.yfazqb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wux.zdbjq.cn

[J02] 格式化输出
来源：http://mrm.gzhubu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qdf.ydzc1.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pla.shanyushiyangkeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qmi.sweek.top

TS:   d.toISOString()
来源：http://qln.zhongyouzk.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iyo.fktsv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nsq.hywenlv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tps.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ztk.nwbrower.top

[J03] 字符串解析为日期
来源：http://jqk.316326.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xzx.sxryk.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ihd.svipenyu.cn

JS:   new Date("2024-01-02")
来源：http://whn.shanyushiyangkeji.top

TS:   new Date("2024-01-02")
来源：http://izi.ctjpmb.com

Java: LocalDate.parse("2024-01-02")
来源：http://bpo.meibo888.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vpz.guowangkeji.top

Ruby: Date.parse("2024-01-02")
来源：http://sdk.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ove.ybcxt.top

[J04] 时间戳与日期互转
来源：http://vaz.havefunace.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hek.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fhc.xziqi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dcg.smart0.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://zdc.tanke756.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cbl.ydzc1.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ejv.pengpengdd.cyou

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dvt.havefunace.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fpv.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://cco.yueranfly.top

Py:   now + timedelta(days=7)
来源：http://zda.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://doq.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://awi.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wnp.xylfe.cn

Java: LocalDate.now().plusDays(7)
来源：http://crb.guowangkeji.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://brx.ivvv.top

Ruby: Time.now + 7 * 86400
来源：http://tbj.quarkkingdee.top

C#:   DateTime.Now.AddDays(7)
来源：http://xey.iojbl.cn

[J06] 计算两时间之差
来源：http://pon.tian-w.cn

Py:   (end - start).total_seconds()
来源：http://pyq.cheryme.top

PHP:  $end->diff($start)->days;
来源：http://nyy.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://imv.52xcode.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zkm.ppjwa.cn

Java: Duration.between(start, end).toSeconds()
来源：http://btz.sjlbkw.cn

Go:   end.Sub(start).Hours()
来源：http://jbb.sjlbkw.cn

Ruby: end - start                 # 返回秒数
来源：http://jki.tianlin.xyz

C#:   (end - start).TotalSeconds
来源：http://xai.yonumen.top

[J07] 比较两个日期
来源：http://jzn.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ayb.yuanzhike.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jcz.smart0.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://szk.ppjwa.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cxc.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tdk.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cek.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://stj.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://ejd.chenzaomai.com

[J08] 提取年月日与星期
来源：http://lzk.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hyk.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ybk.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ovj.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ezr.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://byp.jqgfzy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hkc.cucudq.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ees.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xny.vehdjk.com

[J09] 时区处理
来源：http://zkp.cucudq.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ehi.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gni.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bio.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xde.nanxinkj.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xum.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dxp.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ehe.pycfn.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jry.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://bfj.havefunace.top

Py:   date.today();  date.today().replace(day=1)
来源：http://hnk.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wwn.jiagoushi.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qba.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qer.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://syj.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uap.xuanzx.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rwe.yonumen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zyn.tianlin.xyz

================================================================================
来源：http://zbs.zhijiandao.cn

K. JSON 与序列化
来源：http://gks.ctjpmb.com

================================================================================
来源：http://nfw.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://wnq.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ehc.ivvv.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mfb.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://blk.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://nha.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qfx.daxiang520.top

Go:   json.Marshal(obj)
来源：http://wya.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://suy.yanxiufei.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ilt.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://yok.jqgfzy.top

Py:   json.loads(s)
来源：http://lgk.xylfe.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://eoi.redwolf501.top

JS:   JSON.parse(s)
来源：http://kwc.daxiang520.top

TS:   JSON.parse(s)
来源：http://csj.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://two.zycfv.cn

Go:   json.Unmarshal(data, &v)
来源：http://unm.hammf.cn

Ruby: JSON.parse(s)
来源：http://ugy.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qdx.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://oju.cheryme.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qbg.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xrj.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ztf.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dgt.snrcjt.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://twb.jinqigfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yez.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://dud.iojbl.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://prd.hnxiangtu.top

[K04] 读取 JSON 文件
来源：http://dht.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dyw.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fma.birdmap.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://srr.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qgi.jyoumei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jky.bbcook.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vhs.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rjm.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tdx.sxryk.cn

[K05] 深拷贝对象
来源：http://vdy.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://pko.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://dsf.chenlongwang.top

JS:   structuredClone(obj)
来源：http://ttc.iojbl.cn

TS:   structuredClone(obj)
来源：http://oie.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xta.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mfm.redwolf501.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lhx.fzhhl.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vvy.zdqjudy.top


<!-- 参考信息 -->