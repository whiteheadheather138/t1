代发 wailian999

JS:   class MyError extends Error {}
来源：http://cpi.yj20258888.top

TS:   class MyError extends Error {}
来源：http://jjo.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://rtp.jiagoushi.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hct.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://dxh.ivvv.top

C#:   class MyException : Exception {}
来源：http://xhg.chenjidiqi.icu

[H05] 捕获特定类型
来源：http://hiu.jinqigfzy.top

Py:   except ValueError as e:
来源：http://dwy.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://btd.shanyushiyangkeji.top

JS:   if (e instanceof TypeError) {}
来源：http://fsu.c1oappe.top

TS:   if (e instanceof TypeError) {}
来源：http://pbg.tarul.cn

Java: catch (IOException | SQLException e) {}
来源：http://pvb.aizwys.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yfp.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://mof.zhixingplan.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wzd.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://fkn.daria6918.cn

Py:   value = d.get("k") or default
来源：http://wcp.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://sqb.fanxiaobao.xyz

JS:   obj?.a?.b;  d ?? default
来源：http://tub.tanke756.top

TS:   obj?.a?.b;  d ?? default
来源：http://jop.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wej.vqdsnc.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jiq.cashguo.top

Ruby: d&.dig(:a, :b)
来源：http://psy.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://nqq.ctjpmb.com

[H07] 断言
来源：http://jvo.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://off.pycfn.com

PHP:  assert($x > 0);
来源：http://jhs.yueranfly.top

JS:   console.assert(x > 0);
来源：http://xox.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://yev.iojbl.cn

Java: assert x > 0 : "必须为正";
来源：http://fml.9152youxi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oav.sufxvd.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sgw.cheryme.top

C#:   Debug.Assert(x > 0);
来源：http://scb.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://bea.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://afl.yongpay.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pes.chenzaomai.com

JS:   e.message;  e.stack
来源：http://jhi.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tck.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tez.9152youxi.cn

Go:   err.Error()
来源：http://tya.yueranfly.top

Ruby: e.message;  e.backtrace
来源：http://ukm.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://ngv.sufxvd.cn

[H09] 带错误码的异常
来源：http://nsa.hesvh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vum.fzhhl.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bxj.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://plk.hfpthk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hpu.ybcxt.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vet.smart0.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://npt.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://xph.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ned.gzhubu.top

[H10] 资源自动释放
来源：http://jgf.shzxlz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://khg.fehbvm.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://avt.epnwcf.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lyl.hesvh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rkz.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nxe.yuxming.cn

Go:   defer f.Close()
来源：http://lun.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rcw.vqdsnc.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pmx.yj20258.top

================================================================================
来源：http://oih.cdnleiting.top

I. 正则表达式
来源：http://lvf.316326.xyz

================================================================================
来源：http://uhz.meibo888.top

[I01] 判断是否匹配
来源：http://ztk.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rfs.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://lmy.uphjek.com

JS:   /\d+/.test(s)
来源：http://aeb.aibaodan.cn

TS:   /\d+/.test(s)
来源：http://fir.sxryk.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wao.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://owm.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://ypf.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bba.9152youxi.cn

[I02] 提取所有匹配
来源：http://jvl.xziqi.cn

Py:   re.findall(r"\d+", s)
来源：http://hlv.quarkkingdee.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zdy.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lrw.vehdjk.com

TS:   s.match(/\d+/g)
来源：http://cju.ybcxt.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://boi.yj20258888.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yjo.guowangkeji.top

Ruby: s.scan(/\d+/)
来源：http://pse.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ots.yongpay.top

[I03] 提取捕获分组
来源：http://obh.wangdashe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://say.tian-w.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vhv.yj202588.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lkb.xziqi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vid.xuetiantiany.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tei.cheryme.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mim.zhaomingkeji.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gvz.hesvh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://egg.bjfxy.top

[I04] 正则替换
来源：http://ykv.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bsb.svipenyu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ske.feifeiyinyue.top

JS:   s.replace(/\d+/g, "#")
来源：http://bkj.yonumen.top

TS:   s.replace(/\d+/g, "#")
来源：http://xhk.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://bvq.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://ssq.ybcxt.top

Ruby: s.gsub(/\d+/, "#")
来源：http://wlw.jlsjyb.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ipz.pengpengdd.cyou

[I05] 按正则拆分
来源：http://hkh.yangfankeji.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ynz.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vte.wangdashe.top

JS:   s.split(/\s*,\s*/)
来源：http://euq.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://fhc.zdbjq.cn

Java: s.split("\\s*,\\s*")
来源：http://ztn.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rki.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://gpd.feifeiyinyue.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dtr.snrcjt.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bib.jinqigfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bdl.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lel.jinqigufen.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://drx.mhx1999.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uxh.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wfa.hfpthk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dks.sysykeji.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uhm.quarkkingdee.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qhd.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://rts.chenzaomai.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qtg.dianchejie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gvv.jinqigfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mfo.xinyue.icu

TS:   /error/gim
来源：http://hlz.ivvv.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xiq.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dgl.gogol.net.cn

Ruby: s.scan(/error/i)
来源：http://kvs.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gsu.hammf.cn

[I08] 贪婪与非贪婪匹配
来源：http://rgq.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aui.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pfz.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wlj.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vfq.52xcode.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kzr.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fhd.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rvm.zhoulong.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ufa.cqqwz.cn

================================================================================
来源：http://fgs.vqdsnc.cn

J. 日期与时间
来源：http://fxl.hnqzz.top

================================================================================
来源：http://ldj.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://njy.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rvf.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pvk.xuanzx.com

JS:   new Date();  Date.now()
来源：http://wuh.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://czh.yuanzhike.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hhe.zhengqikj.top

Go:   time.Now()
来源：http://zhw.zhoulong.xyz

Ruby: Time.now
来源：http://maf.gzhubu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nli.fktsv.cn

[J02] 格式化输出
来源：http://bey.ctjpmb.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ier.cashguo.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dha.meibo888.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yuu.daria6918.cn

TS:   d.toISOString()
来源：http://uuf.daxiang520.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bzn.guannengcc.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kez.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wuj.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jon.meibo888.top

[J03] 字符串解析为日期
来源：http://zdz.jiagoushi.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nsv.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zaa.wangshuangyany.cn

JS:   new Date("2024-01-02")
来源：http://xxp.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://snn.cqqwz.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bzb.guannengcc.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kfp.dashuyun.cn

Ruby: Date.parse("2024-01-02")
来源：http://kvf.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fjn.yj20258888.top

[J04] 时间戳与日期互转
来源：http://jje.hnqzz.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hes.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iuz.xylfe.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yyx.0kj1m.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mcw.yangfankeji.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qgy.jinqigufen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qbw.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lxo.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://coz.sufxvd.cn

[J05] 时间加减（加 7 天）
来源：http://nba.mhx1999.top

Py:   now + timedelta(days=7)
来源：http://geq.chenjidiqi.icu

PHP:  (new DateTime())->modify("+7 days");
来源：http://ogg.nwbrower.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tsr.cqqwz.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xuc.wangshuangyany.cn

Java: LocalDate.now().plusDays(7)
来源：http://hym.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ayf.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://spl.yj202588.top

C#:   DateTime.Now.AddDays(7)
来源：http://bps.yj20258.top

[J06] 计算两时间之差
来源：http://lbp.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://edl.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://ytt.daxiang520.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nyy.aizwys.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kis.fanxiaobao.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://ezu.yangfankeji.com

Go:   end.Sub(start).Hours()
来源：http://aeg.cucudq.cn

Ruby: end - start                 # 返回秒数
来源：http://hvm.birdmap.top

C#:   (end - start).TotalSeconds
来源：http://kqx.zhixingplan.top

[J07] 比较两个日期
来源：http://fie.smart0.xyz

Py:   d1 < d2;  d1 == d2
来源：http://jic.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ooz.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://zgv.yj20258.top

TS:   d1.getTime() < d2.getTime()
来源：http://gua.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sfv.ywan-chungtsiang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wac.yfazqb.com

Ruby: d1 < d2;  d1 == d2
来源：http://wte.jinyuanbaomall.cn

C#:   d1 < d2;  d1 == d2
来源：http://gcd.snrcjt.cn

[J08] 提取年月日与星期
来源：http://oyj.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jqe.jianghu66.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ceb.mhx1999.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rzk.ivvv.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jxq.bjfxy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hpo.zhoulong.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yup.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ytw.smart0.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ulk.fanxiaobao.xyz

[J09] 时区处理
来源：http://yvs.sjlbkw.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fcd.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://shu.yvedp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://crh.fehbvm.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jxt.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mun.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lis.sxryk.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kcl.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://atl.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://ybl.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lpb.birdmap.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mgk.jyoumei.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://seh.zdbjq.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ayv.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bqm.tarul.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nhg.daria6918.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://eqv.yj20258.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jzy.cheryme.top

================================================================================
来源：http://djo.zhengqikj.top

K. JSON 与序列化
来源：http://art.zhijiandao.cn

================================================================================
来源：http://elh.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://opk.hcnkem.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kpj.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://snc.sxryk.cn

JS:   JSON.stringify(obj)
来源：http://rpd.zdbjq.cn

TS:   JSON.stringify(obj)
来源：http://xxl.jinyuanbaomall.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tqg.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://wud.nwbrower.top

Ruby: obj.to_json                                     // require "json"
来源：http://nib.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mey.hywenlv.cn

[K02] JSON 字符串转对象
来源：http://hji.jiagoushi.top

Py:   json.loads(s)
来源：http://utu.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ldt.ctjpmb.com

JS:   JSON.parse(s)
来源：http://kcd.gogol.net.cn

TS:   JSON.parse(s)
来源：http://nzt.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kyb.shanyushiyangtech.top

Go:   json.Unmarshal(data, &v)
来源：http://dxy.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://doh.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ygu.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://taj.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zvv.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wvo.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://ztk.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fou.birdmap.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uuv.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ypz.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://stv.jqgfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iet.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://glw.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gkt.tarul.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nvc.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hfo.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://csl.havefunace.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://brs.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vui.ybcxt.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tgx.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ucd.jianghu66.top

[K05] 深拷贝对象
来源：http://uum.guowangkeji.top

Py:   copy.deepcopy(obj)
来源：http://nhe.yvedp.cn

PHP:  unserialize(serialize($obj));
来源：http://qrn.shuidangran.top

JS:   structuredClone(obj)
来源：http://rrf.gogol.net.cn

TS:   structuredClone(obj)
来源：http://heo.dianchejie.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vjw.jinyuanbaomall.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mcj.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dmt.tarul.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bum.bjfxy.top

[K06] 解析 URL 查询串
来源：http://hwf.nanxuanxn.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ffe.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hut.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dfn.xingfuxueyuan.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wvb.yanxiufei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tyx.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vyq.shanyushiyangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cgu.gaohongyu789.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zhp.dianchejie.cn

[K07] 进制转换
来源：http://mgi.ivvv.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://our.ywan-chungtsiang.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jej.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://icv.xuanzx.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ckh.zhongyouzk.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bqt.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tvs.nwbrower.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tzn.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gga.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://qkc.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://ucc.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tnr.feifeiyinyue.top

JS:   v8.serialize(obj)        // Node
来源：http://qqn.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://uqr.ydzc1.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wzc.ybcxt.top


<!-- 参考信息 -->