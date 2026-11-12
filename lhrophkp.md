代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rtf.meibo888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eqz.jqgfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kju.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://krc.sysykeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zmc.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zqe.cashguo.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rqe.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://qvp.jyoumei.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ozf.fzhhl.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ddn.hnqzz.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rba.redwolf501.top

TS:   try { f(); } finally { cleanup(); }
来源：http://cio.andypj.xyz

Java: try { f(); } finally { cleanup(); }
来源：http://ggk.daria6918.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gsn.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://coz.ctjpmb.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://lcb.yuxming.cn

[H03] 主动抛出异常
来源：http://knd.dianchejie.cn

Py:   raise ValueError("错误信息")
来源：http://cjs.yangfankeji.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mlc.zhongyouzk.top

JS:   throw new Error("错误信息");
来源：http://tqp.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://klk.svipenyu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dpg.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eee.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://sjh.vehdjk.com

C#:   throw new ArgumentException("错误信息");
来源：http://aeg.ywan-chungtsiang.top

[H04] 自定义异常类型
来源：http://rym.daria6918.cn

Py:   class MyError(Exception): pass
来源：http://huc.zdqjudy.top

PHP:  class MyError extends RuntimeException {}
来源：http://pvu.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://hcu.xinyue.icu

TS:   class MyError extends Error {}
来源：http://hzg.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://rea.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ptk.yj202588.top

Ruby: class MyError < StandardError; end
来源：http://cxw.ydzc1.top

C#:   class MyException : Exception {}
来源：http://rxb.zdbjq.cn

[H05] 捕获特定类型
来源：http://cun.yj20258.top

Py:   except ValueError as e:
来源：http://hil.xuetiantiany.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ghv.zhiwuduotai.top

JS:   if (e instanceof TypeError) {}
来源：http://vlq.shanyushiyangkeji.top

TS:   if (e instanceof TypeError) {}
来源：http://qxx.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://pvb.yj20258888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://apg.cqqwz.cn

Ruby: rescue ArgumentError => e
来源：http://psd.yangfankeji.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ymv.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://qpx.bbcook.cn

Py:   value = d.get("k") or default
来源：http://srz.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yot.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://aze.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://yxi.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sbh.meibo888.top

Go:   if v, ok := m["k"]; ok { }
来源：http://wae.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://gnb.guannengcc.top

C#:   obj?.A?.B ?? default
来源：http://gmr.shanyushiyangtech.top

[H07] 断言
来源：http://myz.sufxvd.cn

Py:   assert x > 0, "必须为正"
来源：http://obc.tanke756.top

PHP:  assert($x > 0);
来源：http://hmx.cucudq.cn

JS:   console.assert(x > 0);
来源：http://nfv.wangshuangyany.cn

TS:   console.assert(x > 0);
来源：http://vrr.hywenlv.cn

Java: assert x > 0 : "必须为正";
来源：http://qhi.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uvf.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tls.zhaomingkeji.xyz

C#:   Debug.Assert(x > 0);
来源：http://hrj.sufxvd.cn

[H08] 获取错误信息与堆栈
来源：http://poq.hnxiangtu.top

Py:   str(e);  traceback.format_exc()
来源：http://gwi.andypj.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hmm.cashguo.top

JS:   e.message;  e.stack
来源：http://eck.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://agv.wangdashe.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jcn.daria6918.cn

Go:   err.Error()
来源：http://tts.tian-w.cn

Ruby: e.message;  e.backtrace
来源：http://fvs.gotoacloud.top

C#:   e.Message;  e.StackTrace
来源：http://ipl.hammf.cn

[H09] 带错误码的异常
来源：http://aed.zhiwuduotai.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fqc.hnqzz.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fbf.sufxvd.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kkh.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jdj.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ocd.chenlongwang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bto.zhengqikj.top

Ruby: raise MyError.new("fail", 500)
来源：http://gmm.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aqi.andypj.xyz

[H10] 资源自动释放
来源：http://fqk.ivvv.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cuk.ydzc1.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jdj.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gou.yvedp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nby.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://meh.hysaishi.cn

Go:   defer f.Close()
来源：http://fqv.hesvh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fzd.hywenlv.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hcp.ctjpmb.com

================================================================================
来源：http://imh.hnqzz.top

I. 正则表达式
来源：http://ghi.0kj1m.cn

================================================================================
来源：http://muj.epnwcf.com

[I01] 判断是否匹配
来源：http://wof.vehdjk.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://olu.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://loc.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://ypd.yuxming.cn

TS:   /\d+/.test(s)
来源：http://sfc.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gol.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://unf.gaohongyu789.top

Ruby: s.match?(/\d+/)
来源：http://svq.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bcs.guannengcc.top

[I02] 提取所有匹配
来源：http://uju.dashuyun.cn

Py:   re.findall(r"\d+", s)
来源：http://kkf.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kom.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wfx.fengsongda.top

TS:   s.match(/\d+/g)
来源：http://mks.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yek.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sdd.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://cjj.xylfe.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xjm.yueranfly.top

[I03] 提取捕获分组
来源：http://nae.jlsjyb.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fle.jyoumei.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ffp.9152youxi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vtt.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rjv.jinqigufen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://odg.tarul.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qgo.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nxi.xziqi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lvs.haohaochexian.top

[I04] 正则替换
来源：http://fwp.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ckp.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ldd.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nyz.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://krc.haohaochexian.top

Java: s.replaceAll("\\d+", "#")
来源：http://fqm.iojbl.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ebj.yj20258.top

Ruby: s.gsub(/\d+/, "#")
来源：http://dfz.sjlbkw.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gfq.shanyushiyangtech.top

[I05] 按正则拆分
来源：http://rce.jianghu66.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lab.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ebo.aizwys.cn

JS:   s.split(/\s*,\s*/)
来源：http://dja.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://hxx.feifeiyinyue.top

Java: s.split("\\s*,\\s*")
来源：http://bxu.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tbr.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ptv.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zkp.ppjwa.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xtn.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://iwp.jiagoushi.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://npp.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jtp.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yqe.nwbrower.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://irq.jqgfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zdc.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jcn.chenjidiqi.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qkf.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://jmt.zhiwuduotai.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qiz.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oih.fzhhl.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ssg.tarul.cn

TS:   /error/gim
来源：http://ore.yvedp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://udn.52xcode.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yon.yvedp.cn

Ruby: s.scan(/error/i)
来源：http://byt.hnqzz.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ktc.sweek.top

[I08] 贪婪与非贪婪匹配
来源：http://pes.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dly.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jez.yueranfly.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bgp.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ylu.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://oll.ctjpmb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eex.shzxlz.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hnb.wangdashe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zwn.yanxiufei.cn

================================================================================
来源：http://cql.iojbl.cn

J. 日期与时间
来源：http://cvu.smart0.xyz

================================================================================
来源：http://yua.yuanzhike.top

[J01] 获取当前时间
来源：http://hry.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://fbw.xuanzx.com

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kut.wangdashe.top

JS:   new Date();  Date.now()
来源：http://xsk.hnxiangtu.top

TS:   new Date();  Date.now()
来源：http://kmj.hywenlv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://msb.nwbrower.top

Go:   time.Now()
来源：http://gjo.jinyuanbaomall.cn

Ruby: Time.now
来源：http://nqk.cheryme.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://klf.jianghu66.top

[J02] 格式化输出
来源：http://fdm.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gxh.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vtt.wangdashe.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kci.ivvv.top

TS:   d.toISOString()
来源：http://imo.zdbjq.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pif.aibaodan.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yvw.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nej.hongshengwenyu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kda.feifeiyinyue.top

[J03] 字符串解析为日期
来源：http://ycy.sjlbkw.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rca.jinyuanbaomall.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzv.cucudq.cn

JS:   new Date("2024-01-02")
来源：http://auy.cheryme.top

TS:   new Date("2024-01-02")
来源：http://ljt.jinyuanbaomall.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gsz.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qcv.yvedp.cn

Ruby: Date.parse("2024-01-02")
来源：http://lln.havefunace.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zcx.c1oappe.top

[J04] 时间戳与日期互转
来源：http://bnw.redwolf501.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lzs.0kj1m.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vmp.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yty.iojbl.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://keg.fanxiaobao.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ozk.jlsjyb.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tdj.ywan-chungtsiang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uqi.zhoulong.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oqx.tianlin.xyz

[J05] 时间加减（加 7 天）
来源：http://wgt.chenlongwang.top

Py:   now + timedelta(days=7)
来源：http://cmc.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://gtv.chenjidiqi.icu

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://the.jianghu66.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ktq.sjlbkw.cn

Java: LocalDate.now().plusDays(7)
来源：http://xpc.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://afz.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://pxu.zycfv.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pup.yj20258.top

[J06] 计算两时间之差
来源：http://wkx.hnxiangtu.top

Py:   (end - start).total_seconds()
来源：http://cwg.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://uow.zhoulong.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qzx.sxryk.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://abo.c1oappe.top

Java: Duration.between(start, end).toSeconds()
来源：http://ljz.ywan-chungtsiang.top

Go:   end.Sub(start).Hours()
来源：http://gop.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://pjz.andypj.xyz

C#:   (end - start).TotalSeconds
来源：http://dgk.52xcode.cn

[J07] 比较两个日期
来源：http://zet.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://iig.fanxiaobao.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hiz.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://pnz.bjfxy.top

TS:   d1.getTime() < d2.getTime()
来源：http://dbs.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vtm.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vnr.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://sum.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://bjq.hcnkem.com

[J08] 提取年月日与星期
来源：http://zwf.yuxming.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wcx.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nuo.zhongyouzk.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lqq.birdmap.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ohv.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nad.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://trr.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nyr.vehdjk.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://diz.gzhubu.top

[J09] 时区处理
来源：http://uax.wangshuangyany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://juw.vehdjk.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sug.nanxuanxn.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyt.yonumen.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sny.nanxuanxn.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xap.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://anl.jiagoushi.top

Ruby: Time.now.getlocal("+08:00")
来源：http://spr.zhaomingkeji.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewt.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://ylw.xuanzx.com

Py:   date.today();  date.today().replace(day=1)
来源：http://wpw.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://izv.redwolf501.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zvw.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wdt.aizwys.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zch.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xnm.zhaomingkeji.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://niu.zdqjudy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yjo.xuanzx.com

================================================================================
来源：http://hun.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://hrf.zhongyouzk.top

================================================================================
来源：http://opv.chenlongwang.top

[K01] 对象转 JSON 字符串
来源：http://psg.pycfn.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tor.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uyy.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://gox.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://zfk.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://snb.yongpay.top

Go:   json.Marshal(obj)
来源：http://kmw.jinyuanbaomall.cn

Ruby: obj.to_json                                     // require "json"
来源：http://oqg.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bbk.fehbvm.com

[K02] JSON 字符串转对象
来源：http://ezb.redwolf501.top

Py:   json.loads(s)
来源：http://lny.hywenlv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://axq.bjfxy.top

JS:   JSON.parse(s)
来源：http://vzd.gzhubu.top

TS:   JSON.parse(s)
来源：http://bjv.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mbu.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://xhm.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://dgr.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://plv.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://izq.shzxlz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uba.xuetiantiany.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ptg.nanxuanxn.top

JS:   JSON.stringify(obj, null, 2)
来源：http://uaz.redwolf501.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ilj.yanxiufei.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://opc.nwbrower.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qiz.hcnkem.com

Ruby: JSON.pretty_generate(obj)
来源：http://vtc.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uqs.iojbl.cn

[K04] 读取 JSON 文件
来源：http://zsg.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lcb.haohaochexian.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kue.daria6918.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cqv.jinyuanbaomall.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xyd.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xbz.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://aez.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hjl.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mpl.sxryk.cn

[K05] 深拷贝对象
来源：http://dbu.xingfuxueyuan.xyz

Py:   copy.deepcopy(obj)
来源：http://dqb.pengpengdd.cyou

PHP:  unserialize(serialize($obj));
来源：http://tac.kuanghao11.cn

JS:   structuredClone(obj)
来源：http://dca.tarul.cn

TS:   structuredClone(obj)
来源：http://gcd.guannengcc.top


<!-- 参考信息 -->