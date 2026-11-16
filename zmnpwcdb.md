代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://pra.shanyushiyangkeji.top

[H04] 自定义异常类型
来源：http://xmv.hnxiangtu.top

Py:   class MyError(Exception): pass
来源：http://toq.yonumen.top

PHP:  class MyError extends RuntimeException {}
来源：http://ocz.fzhhl.top

JS:   class MyError extends Error {}
来源：http://rjw.bjfxy.top

TS:   class MyError extends Error {}
来源：http://ael.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://msh.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xbm.ctjpmb.com

Ruby: class MyError < StandardError; end
来源：http://ypf.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://esh.aibaodan.cn

[H05] 捕获特定类型
来源：http://huf.yongpay.top

Py:   except ValueError as e:
来源：http://vkr.jyoumei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lfw.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://tvu.hnxiangtu.top

TS:   if (e instanceof TypeError) {}
来源：http://vwd.jianghu66.top

Java: catch (IOException | SQLException e) {}
来源：http://gik.sweek.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lhz.sjlbkw.cn

Ruby: rescue ArgumentError => e
来源：http://cin.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://prr.chenjidiqi.icu

[H06] 可选值 / 空值安全访问
来源：http://ywr.52xcode.cn

Py:   value = d.get("k") or default
来源：http://sti.xuetiantiany.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qhm.zhengqikj.top

JS:   obj?.a?.b;  d ?? default
来源：http://qis.shanyushiyangtech.top

TS:   obj?.a?.b;  d ?? default
来源：http://esu.aibaodan.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iuj.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lld.jinghuilouyu.cn

Ruby: d&.dig(:a, :b)
来源：http://lmi.gotoacloud.top

C#:   obj?.A?.B ?? default
来源：http://jgl.smart0.xyz

[H07] 断言
来源：http://cpo.nwbrower.top

Py:   assert x > 0, "必须为正"
来源：http://bhp.daxiang520.top

PHP:  assert($x > 0);
来源：http://eyp.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://lvf.quarkkingdee.top

TS:   console.assert(x > 0);
来源：http://uka.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://bnx.shuidangran.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://omp.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://brv.hongshengwenyu.top

C#:   Debug.Assert(x > 0);
来源：http://hde.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://tmh.epnwcf.com

Py:   str(e);  traceback.format_exc()
来源：http://eno.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zeq.yj20258888.top

JS:   e.message;  e.stack
来源：http://zhg.snrcjt.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qeq.vqdsnc.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gas.hfpthk.cn

Go:   err.Error()
来源：http://mvb.tarul.cn

Ruby: e.message;  e.backtrace
来源：http://lks.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://pdk.yj20258.top

[H09] 带错误码的异常
来源：http://ifq.hfpthk.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fuk.snrcjt.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://axx.jqgufenzy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tyq.zycfv.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ycv.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://prt.fktsv.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xie.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://vzc.sxryk.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dhc.ywan-chungtsiang.top

[H10] 资源自动释放
来源：http://rjx.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://rnn.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vem.yj202588.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fnl.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oxg.feifeiyinyue.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nvp.shangyingyoupin.top

Go:   defer f.Close()
来源：http://gff.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yzu.fzhhl.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xhr.jqgufenzy.top

================================================================================
来源：http://kpb.chenzaomai.com

I. 正则表达式
来源：http://jpo.andypj.xyz

================================================================================
来源：http://vpi.aibaodan.cn

[I01] 判断是否匹配
来源：http://obn.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hgf.zhijiandao.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hgk.chenjidiqi.icu

JS:   /\d+/.test(s)
来源：http://dxs.sjlbkw.cn

TS:   /\d+/.test(s)
来源：http://qho.jyoumei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yrv.yonumen.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rza.yj202588.top

Ruby: s.match?(/\d+/)
来源：http://gyd.fengsongda.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hsn.ehwqpu.com

[I02] 提取所有匹配
来源：http://oxn.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://skt.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mrc.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xzh.xziqi.cn

TS:   s.match(/\d+/g)
来源：http://fya.mhx1999.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pqs.snrcjt.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ewl.cqqwz.cn

Ruby: s.scan(/\d+/)
来源：http://nmf.yvedp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://swt.nwbrower.top

[I03] 提取捕获分组
来源：http://dke.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hkq.zhengqikj.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ics.yonumen.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hcm.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://slv.bjfxy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vat.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lrk.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qnz.fzhhl.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nbs.vqdsnc.cn

[I04] 正则替换
来源：http://han.hongshengwenyu.top

Py:   re.sub(r"\d+", "#", s)
来源：http://pkf.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hre.daria6918.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oug.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dli.gogol.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hbo.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://omk.guowangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mfp.yangfankeji.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xte.andypj.xyz

[I05] 按正则拆分
来源：http://hfp.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://lgc.havefunace.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hmy.xziqi.cn

JS:   s.split(/\s*,\s*/)
来源：http://jcb.sxryk.cn

TS:   s.split(/\s*,\s*/)
来源：http://zjp.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://enm.guannengcc.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zdr.jinyuanbaomall.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wjk.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gch.sweek.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ttt.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zpe.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://auo.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xdn.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qjv.aizwys.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rgq.cdnleiting.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://khp.haohaochexian.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rwn.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qvg.zhongyouzk.top

[I07] 忽略大小写与多行模式
来源：http://xsv.tanke756.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vdz.wangdashe.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://isv.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wxc.sysykeji.top

TS:   /error/gim
来源：http://yjz.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lmk.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hvo.ydzc1.top

Ruby: s.scan(/error/i)
来源：http://mbz.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gla.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://ztd.yj202588.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://trj.cucudq.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qoj.hywenlv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://prx.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wgr.jinqigufen.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ysx.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://znn.yonumen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nft.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://aaz.shanyushiyangtech.top

================================================================================
来源：http://fsm.gogol.net.cn

J. 日期与时间
来源：http://nmk.hongshengwenyu.top

================================================================================
来源：http://stp.bbcook.cn

[J01] 获取当前时间
来源：http://qvk.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jki.jianghu66.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gsk.redwolf501.top

JS:   new Date();  Date.now()
来源：http://luo.ivvv.top

TS:   new Date();  Date.now()
来源：http://hjn.haohaochexian.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vsx.jlsjyb.cn

Go:   time.Now()
来源：http://jdu.chenjidiqi.icu

Ruby: Time.now
来源：http://zdq.ctjpmb.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://egw.xingfuxueyuan.xyz

[J02] 格式化输出
来源：http://bnv.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cag.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ccm.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://snb.guannengcc.top

TS:   d.toISOString()
来源：http://pro.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://njd.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://csm.shuidangran.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hxc.nwbrower.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mcf.kuanghao11.cn

[J03] 字符串解析为日期
来源：http://myk.ctjpmb.com

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wqs.ctjpmb.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qnv.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://vaf.gogol.net.cn

TS:   new Date("2024-01-02")
来源：http://qgv.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://edz.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jqg.fehbvm.com

Ruby: Date.parse("2024-01-02")
来源：http://xyr.jinqigfzy.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tyo.fzhhl.top

[J04] 时间戳与日期互转
来源：http://gbr.bjfxy.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fwh.daria6918.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iev.fktsv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rtm.sysykeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://zbk.52xcode.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zxb.shanyushiyangkeji.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wfe.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gll.yuxming.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uwj.jinqigufen.top

[J05] 时间加减（加 7 天）
来源：http://axb.jyoumei.cn

Py:   now + timedelta(days=7)
来源：http://czf.havefunace.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://yan.yanxiufei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vtw.cashguo.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://str.hnxiangtu.top

Java: LocalDate.now().plusDays(7)
来源：http://gwf.zhoulong.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lxg.xingfuxueyuan.xyz

Ruby: Time.now + 7 * 86400
来源：http://jjr.xuetiantiany.cn

C#:   DateTime.Now.AddDays(7)
来源：http://vgv.mhx1999.top

[J06] 计算两时间之差
来源：http://gqg.yfazqb.com

Py:   (end - start).total_seconds()
来源：http://uxd.yanxiufei.cn

PHP:  $end->diff($start)->days;
来源：http://mbh.jqgfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wkx.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zyc.svipenyu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cwb.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://zkg.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://uoa.fktsv.cn

C#:   (end - start).TotalSeconds
来源：http://ich.hongshengwenyu.top

[J07] 比较两个日期
来源：http://tpd.jianghu66.top

Py:   d1 < d2;  d1 == d2
来源：http://bqn.iojbl.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ltl.316326.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://uip.zdqjudy.top

TS:   d1.getTime() < d2.getTime()
来源：http://utc.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://feq.shangyingyoupin.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pmm.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://meu.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://mih.epnwcf.com

[J08] 提取年月日与星期
来源：http://zcp.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yej.xinyue.icu

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pxi.fzhhl.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tdz.yongpay.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pjo.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wgl.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tcd.yanxiufei.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gsa.chenzaomai.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gwe.yj202588.top

[J09] 时区处理
来源：http://xbf.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cwp.cdnleiting.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://doo.fzhhl.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ybo.epnwcf.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sks.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kqt.guannengcc.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bcj.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://kjj.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gtg.hnxiangtu.top

[J10] 取今天 / 本月第一天
来源：http://uui.shzxlz.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://efd.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uce.cheryme.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mmg.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vhd.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cxr.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zgo.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iwv.fehbvm.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jxp.fanxiaobao.xyz

================================================================================
来源：http://pue.cheryme.top

K. JSON 与序列化
来源：http://pkk.ywan-chungtsiang.top

================================================================================
来源：http://jyo.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://gcs.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dgc.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nyh.jinqigufen.top

JS:   JSON.stringify(obj)
来源：http://mzr.yj20258.top

TS:   JSON.stringify(obj)
来源：http://typ.dashuyun.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://iau.bbcook.cn

Go:   json.Marshal(obj)
来源：http://bdm.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://psj.chenjidiqi.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://vie.cucudq.cn

[K02] JSON 字符串转对象
来源：http://csx.quarkkingdee.top

Py:   json.loads(s)
来源：http://jzr.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mmz.pengpengdd.cyou

JS:   JSON.parse(s)
来源：http://cqe.tarul.cn

TS:   JSON.parse(s)
来源：http://zvs.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ijz.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://iit.shanyushiyangtech.top

Ruby: JSON.parse(s)
来源：http://gct.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zhq.zdbjq.cn

[K03] JSON 美化输出（带缩进）
来源：http://spr.tarul.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://auv.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jpw.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://riw.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hem.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bem.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hos.jinqigfzy.top

Ruby: JSON.pretty_generate(obj)
来源：http://kvn.xuanzx.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wnj.jianghu66.top

[K04] 读取 JSON 文件
来源：http://vqc.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wcv.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gbe.shzxlz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qcy.cheryme.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nsp.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fil.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ile.yuxming.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ysz.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://koa.yongpay.top

[K05] 深拷贝对象
来源：http://vjo.zhoulong.xyz

Py:   copy.deepcopy(obj)
来源：http://rju.shzxlz.cn

PHP:  unserialize(serialize($obj));
来源：http://qeu.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://gtc.zhixingplan.top

TS:   structuredClone(obj)
来源：http://nqm.ivvv.top

Java: // 手写拷贝构造，或序列化往返
来源：http://uqt.zhiwuduotai.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://noz.chenjidiqi.icu

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fjo.yj20258888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://pic.sxryk.cn

[K06] 解析 URL 查询串
来源：http://jmj.zhiwuduotai.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wdv.guowangkeji.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jak.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mah.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ttq.chenjidiqi.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tjv.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://blu.dianchejie.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xxr.xingfuxueyuan.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ueo.epnwcf.com

[K07] 进制转换
来源：http://vqz.gogol.net.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://udk.nanxinkj.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yxd.cucudq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mtg.yj20258.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pvv.hesvh.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gpz.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dgr.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pdf.ydzc1.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gwt.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://kzu.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://chg.daxiang520.top


<!-- 参考信息 -->