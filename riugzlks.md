代发 wailian999

TS:   throw new Error("错误信息");
来源：http://edi.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zxz.zhijiandao.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eig.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://uaq.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://fak.chenzaomai.com

[H04] 自定义异常类型
来源：http://muj.xuetiantiany.cn

Py:   class MyError(Exception): pass
来源：http://qpn.sysykeji.top

PHP:  class MyError extends RuntimeException {}
来源：http://qyn.hesvh.cn

JS:   class MyError extends Error {}
来源：http://gmr.zhijiandao.cn

TS:   class MyError extends Error {}
来源：http://yqj.xingfuxueyuan.xyz

Java: class MyException extends RuntimeException {}
来源：http://tcw.zhengqikj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iep.gotoacloud.top

Ruby: class MyError < StandardError; end
来源：http://fqy.cdnleiting.top

C#:   class MyException : Exception {}
来源：http://ecr.xziqi.cn

[H05] 捕获特定类型
来源：http://nci.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://omr.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kub.ybcxt.top

JS:   if (e instanceof TypeError) {}
来源：http://kje.yj20258.top

TS:   if (e instanceof TypeError) {}
来源：http://cub.chenzaomai.com

Java: catch (IOException | SQLException e) {}
来源：http://vkt.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vik.dashuyun.cn

Ruby: rescue ArgumentError => e
来源：http://cip.pengpengdd.cyou

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uov.redwolf501.top

[H06] 可选值 / 空值安全访问
来源：http://sup.yj20258888.top

Py:   value = d.get("k") or default
来源：http://zwy.yuanzhike.top

PHP:  $v = $d["k"] ?? null;
来源：http://dex.ydjk.org.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cmh.hammf.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pww.cucudq.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oeq.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eaq.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://lut.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://zml.tarul.cn

[H07] 断言
来源：http://xvt.quarkkingdee.top

Py:   assert x > 0, "必须为正"
来源：http://mql.yangfankeji.com

PHP:  assert($x > 0);
来源：http://sgh.9152youxi.cn

JS:   console.assert(x > 0);
来源：http://xiq.birdmap.top

TS:   console.assert(x > 0);
来源：http://xcj.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://obr.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jef.zhixingplan.top

Ruby: raise "必须为正" unless x > 0
来源：http://jks.quarkkingdee.top

C#:   Debug.Assert(x > 0);
来源：http://vap.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://ovq.jqgufenzy.top

Py:   str(e);  traceback.format_exc()
来源：http://bjr.redwolf501.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tme.sweek.top

JS:   e.message;  e.stack
来源：http://huq.jlsjyb.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xiq.yj20258.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tfd.xuetiantiany.cn

Go:   err.Error()
来源：http://tpx.guannengcc.top

Ruby: e.message;  e.backtrace
来源：http://ylm.hesvh.cn

C#:   e.Message;  e.StackTrace
来源：http://dpr.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://yvl.yj20258888.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mjg.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://yki.yuxming.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ehw.zdqjudy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yls.52xcode.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dlb.ydzc1.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jwt.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://zlm.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://tgc.xinyue.icu

[H10] 资源自动释放
来源：http://wrj.cheryme.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://oqt.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fcq.xinyue.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uza.daria6918.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gxr.hywenlv.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hvr.nwbrower.top

Go:   defer f.Close()
来源：http://whq.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nhm.tianlin.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oxz.xylfe.cn

================================================================================
来源：http://cwr.zhijiandao.cn

I. 正则表达式
来源：http://qns.jinghuilouyu.cn

================================================================================
来源：http://vmk.zhiwuduotai.top

[I01] 判断是否匹配
来源：http://jin.xuetiantiany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tov.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://cqr.ydzc1.top

JS:   /\d+/.test(s)
来源：http://xpo.mhx1999.top

TS:   /\d+/.test(s)
来源：http://vbg.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qab.tian-w.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bns.zycfv.cn

Ruby: s.match?(/\d+/)
来源：http://ula.gzhubu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nka.cashguo.top

[I02] 提取所有匹配
来源：http://ncv.zhoulong.xyz

Py:   re.findall(r"\d+", s)
来源：http://eok.52xcode.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://idi.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xod.cqqwz.cn

TS:   s.match(/\d+/g)
来源：http://jpq.cheryme.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zkg.yuanzhike.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vcm.kuanghao11.cn

Ruby: s.scan(/\d+/)
来源：http://ysz.redwolf501.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mkj.hcnkem.com

[I03] 提取捕获分组
来源：http://iuf.epnwcf.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pzc.tianlin.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dst.hnqzz.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybr.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qni.chenlongwang.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vaf.shangyingyoupin.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xjt.shzxlz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iqz.hywenlv.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xaj.sxryk.cn

[I04] 正则替换
来源：http://zfo.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rtv.tianlin.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://stq.yj20258.top

JS:   s.replace(/\d+/g, "#")
来源：http://mxi.ybcxt.top

TS:   s.replace(/\d+/g, "#")
来源：http://bwk.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://drh.chenlongwang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zfl.epnwcf.com

Ruby: s.gsub(/\d+/, "#")
来源：http://mcf.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kba.hywenlv.cn

[I05] 按正则拆分
来源：http://tjc.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ndo.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bqb.chenlongwang.top

JS:   s.split(/\s*,\s*/)
来源：http://dyp.xylfe.cn

TS:   s.split(/\s*,\s*/)
来源：http://kqg.yanxiufei.cn

Java: s.split("\\s*,\\s*")
来源：http://lyd.gaohongyu789.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uwe.ivvv.top

Ruby: s.split(/\s*,\s*/)
来源：http://zwo.jqgfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sdb.fktsv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uat.wangdashe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uzp.hcnkem.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uns.c1oappe.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jlu.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cpn.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dfa.hongshengwenyu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pzl.zhengqikj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dau.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rjb.jianghu66.top

[I07] 忽略大小写与多行模式
来源：http://rbl.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kyr.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://czz.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jdy.hfpthk.cn

TS:   /error/gim
来源：http://lqf.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mkv.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mab.zhijiandao.cn

Ruby: s.scan(/error/i)
来源：http://ckw.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://azt.pengpengdd.cyou

[I08] 贪婪与非贪婪匹配
来源：http://vpb.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vkk.chenzaomai.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bwo.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://afj.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rdo.9152youxi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://orc.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rpc.wangdashe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jgy.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jvm.fengsongda.top

================================================================================
来源：http://yik.ydzc1.top

J. 日期与时间
来源：http://dzd.uphjek.com

================================================================================
来源：http://tfm.zhongyouzk.top

[J01] 获取当前时间
来源：http://ykk.gogol.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://evf.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gkd.gzhubu.top

JS:   new Date();  Date.now()
来源：http://yhf.ybcxt.top

TS:   new Date();  Date.now()
来源：http://hab.shuidangran.top

Java: LocalDateTime.now();  Instant.now()
来源：http://uin.ydjk.org.cn

Go:   time.Now()
来源：http://pne.yonumen.top

Ruby: Time.now
来源：http://rdc.yj202588.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rai.shzxlz.cn

[J02] 格式化输出
来源：http://ugw.quarkkingdee.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://woi.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rmp.hesvh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mhd.zdqjudy.top

TS:   d.toISOString()
来源：http://hki.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ids.ivvv.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ycq.vehdjk.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://abd.fengsongda.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://agz.xylfe.cn

[J03] 字符串解析为日期
来源：http://mic.daxiang520.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ntt.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ymx.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://vjf.ywan-chungtsiang.top

TS:   new Date("2024-01-02")
来源：http://tgi.hnxiangtu.top

Java: LocalDate.parse("2024-01-02")
来源：http://uwq.jlsjyb.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://iri.haohaochexian.top

Ruby: Date.parse("2024-01-02")
来源：http://qob.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lkv.feifeiyinyue.top

[J04] 时间戳与日期互转
来源：http://ybu.jinqigufen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://weq.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://acj.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aav.cucudq.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fkt.guowangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ewd.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pfp.ivvv.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ssr.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bfb.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://nrl.hnqzz.top

Py:   now + timedelta(days=7)
来源：http://xub.yuxming.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yvr.fktsv.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bry.0kj1m.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dgx.hammf.cn

Java: LocalDate.now().plusDays(7)
来源：http://plc.aizwys.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hdc.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://ejo.vehdjk.com

C#:   DateTime.Now.AddDays(7)
来源：http://xth.hammf.cn

[J06] 计算两时间之差
来源：http://dhd.guannengcc.top

Py:   (end - start).total_seconds()
来源：http://hdf.52xcode.cn

PHP:  $end->diff($start)->days;
来源：http://hzb.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wcp.andypj.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mbr.cashguo.top

Java: Duration.between(start, end).toSeconds()
来源：http://aog.jiagoushi.top

Go:   end.Sub(start).Hours()
来源：http://fqq.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://zvd.gzhubu.top

C#:   (end - start).TotalSeconds
来源：http://vwv.gotoacloud.top

[J07] 比较两个日期
来源：http://cmt.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://zkv.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hee.pycfn.com

JS:   d1.getTime() < d2.getTime()
来源：http://uma.ehwqpu.com

TS:   d1.getTime() < d2.getTime()
来源：http://voo.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cro.fanxiaobao.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lbp.pycfn.com

Ruby: d1 < d2;  d1 == d2
来源：http://wge.sweek.top

C#:   d1 < d2;  d1 == d2
来源：http://fzt.zhixingplan.top

[J08] 提取年月日与星期
来源：http://exj.chenjidiqi.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ydc.yj20258.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fst.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uoo.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qai.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mrq.fehbvm.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://phf.52xcode.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dsu.cqqwz.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qpn.hongshengwenyu.top

[J09] 时区处理
来源：http://wiw.xuetiantiany.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://eec.jqgufenzy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tiy.52xcode.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wmi.52xcode.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fon.ivvv.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sgm.jianghu66.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jtf.sufxvd.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://pjk.hongshengwenyu.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ncr.tian-w.cn

[J10] 取今天 / 本月第一天
来源：http://iqn.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bvg.nwbrower.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pnb.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mng.gaohongyu789.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iiq.zhongyouzk.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://yiv.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cop.ehwqpu.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://reu.jyoumei.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kgm.hnqzz.top

================================================================================
来源：http://agq.tianlin.xyz

K. JSON 与序列化
来源：http://wtz.hesvh.cn

================================================================================
来源：http://ryh.birdmap.top

[K01] 对象转 JSON 字符串
来源：http://uhd.jqgufenzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tou.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xtj.hfpthk.cn

JS:   JSON.stringify(obj)
来源：http://xgu.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://rox.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wss.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://ouc.feifeiyinyue.top

Ruby: obj.to_json                                     // require "json"
来源：http://ten.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://nuy.nanxinkj.top

[K02] JSON 字符串转对象
来源：http://izw.zhengqikj.top

Py:   json.loads(s)
来源：http://sio.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ove.quarkkingdee.top

JS:   JSON.parse(s)
来源：http://ukr.uphjek.com

TS:   JSON.parse(s)
来源：http://mhp.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pby.cheryme.top

Go:   json.Unmarshal(data, &v)
来源：http://mxz.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://cgv.xinyue.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gky.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://swp.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://htr.zhixingplan.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lpf.tarul.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fmk.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://izw.vqdsnc.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nzn.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uiw.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tvf.pycfn.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jql.ydzc1.top

[K04] 读取 JSON 文件
来源：http://fao.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://caa.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iny.nanxinkj.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://laf.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynu.jinqigfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ljz.chenlongwang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ydi.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://eds.yvedp.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yft.cheryme.top

[K05] 深拷贝对象
来源：http://krl.xziqi.cn

Py:   copy.deepcopy(obj)
来源：http://yzy.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://vlc.nwbrower.top

JS:   structuredClone(obj)
来源：http://jfr.9152youxi.cn

TS:   structuredClone(obj)
来源：http://bwp.hcnkem.com

Java: // 手写拷贝构造，或序列化往返
来源：http://sjn.chenzaomai.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hbg.nanxuanxn.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://azy.nanxuanxn.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ppb.hesvh.cn

[K06] 解析 URL 查询串
来源：http://pkj.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ohl.zhengqikj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hbj.cheryme.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gls.cashguo.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wuw.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ime.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nhg.xingfuxueyuan.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://red.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sme.fehbvm.com

[K07] 进制转换
来源：http://apr.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://pyb.hnxiangtu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gtp.gaohongyu789.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zlk.pycfn.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fng.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mya.uphjek.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ewr.ybcxt.top


<!-- 参考信息 -->