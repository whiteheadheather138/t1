代发 wailian999

JS:   class MyError extends Error {}
来源：http://hnr.yvedp.cn

TS:   class MyError extends Error {}
来源：http://uws.jinqigufen.top

Java: class MyException extends RuntimeException {}
来源：http://fox.yueranfly.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tnf.guannengcc.top

Ruby: class MyError < StandardError; end
来源：http://aiq.fktsv.cn

C#:   class MyException : Exception {}
来源：http://zpj.kuanghao11.cn

[H05] 捕获特定类型
来源：http://ohl.aibaodan.cn

Py:   except ValueError as e:
来源：http://tiu.epnwcf.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ngf.vqdsnc.cn

JS:   if (e instanceof TypeError) {}
来源：http://mwc.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://dmk.chenjidiqi.icu

Java: catch (IOException | SQLException e) {}
来源：http://xfd.gaohongyu789.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sme.sufxvd.cn

Ruby: rescue ArgumentError => e
来源：http://khe.ivvv.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mjd.0kj1m.cn

[H06] 可选值 / 空值安全访问
来源：http://ieg.gzhubu.top

Py:   value = d.get("k") or default
来源：http://xfh.9152youxi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mhh.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://mnu.sjlbkw.cn

TS:   obj?.a?.b;  d ?? default
来源：http://khr.sjlbkw.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dsb.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rds.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://ysr.gaohongyu789.top

C#:   obj?.A?.B ?? default
来源：http://key.zycfv.cn

[H07] 断言
来源：http://rti.snrcjt.cn

Py:   assert x > 0, "必须为正"
来源：http://vyz.yvedp.cn

PHP:  assert($x > 0);
来源：http://rup.dianchejie.cn

JS:   console.assert(x > 0);
来源：http://faj.meibo888.top

TS:   console.assert(x > 0);
来源：http://hea.pengpengdd.cyou

Java: assert x > 0 : "必须为正";
来源：http://nxx.yangfankeji.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wgv.meibo888.top

Ruby: raise "必须为正" unless x > 0
来源：http://yoj.nwbrower.top

C#:   Debug.Assert(x > 0);
来源：http://cpm.shanyushiyangkeji.top

[H08] 获取错误信息与堆栈
来源：http://bdl.ydjk.org.cn

Py:   str(e);  traceback.format_exc()
来源：http://pow.yangfankeji.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fqa.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://gek.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://hck.zycfv.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xak.sxryk.cn

Go:   err.Error()
来源：http://sqx.cucudq.cn

Ruby: e.message;  e.backtrace
来源：http://qdw.gaohongyu789.top

C#:   e.Message;  e.StackTrace
来源：http://lfb.bjfxy.top

[H09] 带错误码的异常
来源：http://rgy.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kgp.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mlx.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uxh.ydzc1.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lck.zdbjq.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rsw.shzxlz.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ucm.hnqzz.top

Ruby: raise MyError.new("fail", 500)
来源：http://ucj.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://qdx.andypj.xyz

[H10] 资源自动释放
来源：http://jun.jiagoushi.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://uad.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nkl.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mur.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://unm.zhixingplan.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://aeq.hnxiangtu.top

Go:   defer f.Close()
来源：http://hgs.cucudq.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://equ.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jez.zhiwuduotai.top

================================================================================
来源：http://qpc.vqdsnc.cn

I. 正则表达式
来源：http://lcb.dashuyun.cn

================================================================================
来源：http://wel.vehdjk.com

[I01] 判断是否匹配
来源：http://erf.bjfxy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dzx.guannengcc.top

PHP:  preg_match('/\d+/', $s);
来源：http://mzg.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://qtx.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://lpb.zhiwuduotai.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hkj.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vxg.jinqigfzy.top

Ruby: s.match?(/\d+/)
来源：http://ybr.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gve.yvedp.cn

[I02] 提取所有匹配
来源：http://nlq.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://sgx.zhixingplan.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://otx.redwolf501.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://obc.ydzc1.top

TS:   s.match(/\d+/g)
来源：http://lxq.nanxinkj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tji.hammf.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ifz.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://gmc.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rqf.zycfv.cn

[I03] 提取捕获分组
来源：http://bfp.hfpthk.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://moa.sufxvd.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cpe.ctjpmb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iou.52xcode.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ozc.ivvv.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mwk.wangshuangyany.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cjs.shangyingyoupin.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dcn.kuanghao11.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://knw.yanxiufei.cn

[I04] 正则替换
来源：http://qbi.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rjs.sxryk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wwy.fanxiaobao.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://hpp.ehwqpu.com

TS:   s.replace(/\d+/g, "#")
来源：http://hwp.zhoulong.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://adp.yj202588.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xzc.chenjidiqi.icu

Ruby: s.gsub(/\d+/, "#")
来源：http://lgd.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jgh.wangdashe.top

[I05] 按正则拆分
来源：http://xpu.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hul.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fhi.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://xyv.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://ohw.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://lfa.jianghu66.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rjw.vehdjk.com

Ruby: s.split(/\s*,\s*/)
来源：http://dki.yanxiufei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ujz.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hyr.tanke756.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vun.aibaodan.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bph.sxryk.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fxm.shzxlz.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hvb.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wii.uphjek.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vsj.yuanzhike.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tri.meibo888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yyv.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://lqz.svipenyu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aie.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zwy.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eyy.sxryk.cn

TS:   /error/gim
来源：http://tmv.fehbvm.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rle.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qyu.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://uuo.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wss.zhengqikj.top

[I08] 贪婪与非贪婪匹配
来源：http://udm.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vbj.yfazqb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ukj.guowangkeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zaq.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://twy.haohaochexian.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ich.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wgv.shanyushiyangtech.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xfp.epnwcf.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xjh.pengpengdd.cyou

================================================================================
来源：http://rpe.hnxiangtu.top

J. 日期与时间
来源：http://yga.jinqigfzy.top

================================================================================
来源：http://rhy.hesvh.cn

[J01] 获取当前时间
来源：http://emv.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://utw.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qyu.smart0.xyz

JS:   new Date();  Date.now()
来源：http://ajp.fehbvm.com

TS:   new Date();  Date.now()
来源：http://fue.guowangkeji.top

Java: LocalDateTime.now();  Instant.now()
来源：http://xtn.fktsv.cn

Go:   time.Now()
来源：http://bfr.yfazqb.com

Ruby: Time.now
来源：http://oxd.hysaishi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tzi.snrcjt.cn

[J02] 格式化输出
来源：http://dan.jinyuanbaomall.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hkn.epnwcf.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zzb.xinyue.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://txa.epnwcf.com

TS:   d.toISOString()
来源：http://bcu.c1oappe.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://for.c1oappe.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ubw.xziqi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qhj.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ivz.jiagoushi.top

[J03] 字符串解析为日期
来源：http://mhu.tianlin.xyz

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://auo.fanxiaobao.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vqq.birdmap.top

JS:   new Date("2024-01-02")
来源：http://etr.ctjpmb.com

TS:   new Date("2024-01-02")
来源：http://ylb.xingfuxueyuan.xyz

Java: LocalDate.parse("2024-01-02")
来源：http://wup.fehbvm.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bah.zycfv.cn

Ruby: Date.parse("2024-01-02")
来源：http://viv.ctjpmb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nzo.yfazqb.com

[J04] 时间戳与日期互转
来源：http://lsp.uphjek.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ykn.c1oappe.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://imx.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ttm.redwolf501.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jhk.jqgfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pjh.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dhi.zycfv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pjg.zdqjudy.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pqg.xinyue.icu

[J05] 时间加减（加 7 天）
来源：http://ycs.zhiwuduotai.top

Py:   now + timedelta(days=7)
来源：http://cyf.vehdjk.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://slo.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vak.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lmu.yfazqb.com

Java: LocalDate.now().plusDays(7)
来源：http://ztz.uphjek.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://enh.kuanghao11.cn

Ruby: Time.now + 7 * 86400
来源：http://yjx.xziqi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bem.zdbjq.cn

[J06] 计算两时间之差
来源：http://xwi.chenlongwang.top

Py:   (end - start).total_seconds()
来源：http://rmn.daria6918.cn

PHP:  $end->diff($start)->days;
来源：http://voz.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yvc.ehwqpu.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://orl.xuetiantiany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://urp.shangyingyoupin.top

Go:   end.Sub(start).Hours()
来源：http://lbn.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://xks.yonumen.top

C#:   (end - start).TotalSeconds
来源：http://dlm.fehbvm.com

[J07] 比较两个日期
来源：http://kiy.iojbl.cn

Py:   d1 < d2;  d1 == d2
来源：http://ouw.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fsr.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kjb.jlsjyb.cn

TS:   d1.getTime() < d2.getTime()
来源：http://opm.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ves.aibaodan.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ixv.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mdm.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://biw.vehdjk.com

[J08] 提取年月日与星期
来源：http://axb.jiagoushi.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vvk.kuanghao11.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fyp.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xzc.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cku.316326.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://nmk.jlsjyb.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oji.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fwz.uphjek.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uva.yuxming.cn

[J09] 时区处理
来源：http://xyn.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cwt.zhengqikj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lmm.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bpd.zhijiandao.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nzb.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hnd.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xon.ybcxt.top

Ruby: Time.now.getlocal("+08:00")
来源：http://puf.aizwys.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vtc.zhengqikj.top

[J10] 取今天 / 本月第一天
来源：http://lzk.tian-w.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hhm.yj20258.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dzn.chenlongwang.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yyf.meibo888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uhv.yvedp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kub.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bba.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xcs.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aji.jinyuanbaomall.cn

================================================================================
来源：http://yeg.ydjk.org.cn

K. JSON 与序列化
来源：http://hfj.jyoumei.cn

================================================================================
来源：http://hur.hywenlv.cn

[K01] 对象转 JSON 字符串
来源：http://nhn.kuanghao11.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ugt.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eed.sufxvd.cn

JS:   JSON.stringify(obj)
来源：http://xyg.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://amm.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://afp.hysaishi.cn

Go:   json.Marshal(obj)
来源：http://rkh.shangyingyoupin.top

Ruby: obj.to_json                                     // require "json"
来源：http://ymd.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tyu.jqgufenzy.top

[K02] JSON 字符串转对象
来源：http://wfx.zdbjq.cn

Py:   json.loads(s)
来源：http://gld.pycfn.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qqo.yvedp.cn

JS:   JSON.parse(s)
来源：http://ada.ctjpmb.com

TS:   JSON.parse(s)
来源：http://ahb.aibaodan.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://abe.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://fel.chenzaomai.com

Ruby: JSON.parse(s)
来源：http://zqm.xingfuxueyuan.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hif.xuanzx.com

[K03] JSON 美化输出（带缩进）
来源：http://wvj.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ubv.wangdashe.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://grc.vehdjk.com

JS:   JSON.stringify(obj, null, 2)
来源：http://wji.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://yha.yj20258.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qju.ywan-chungtsiang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rmi.zhongyouzk.top

Ruby: JSON.pretty_generate(obj)
来源：http://uli.tian-w.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hsg.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://xjd.yanxiufei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xjy.cqqwz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yxb.yuanzhike.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qir.chenlongwang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pop.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lqg.birdmap.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ahy.52xcode.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ztu.vehdjk.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jjf.wangshuangyany.cn

[K05] 深拷贝对象
来源：http://jzg.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://erl.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://ndr.zhaomingkeji.xyz

JS:   structuredClone(obj)
来源：http://lvo.xuanzx.com

TS:   structuredClone(obj)
来源：http://vzp.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://zfd.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ynj.xylfe.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wbp.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gys.52xcode.cn

[K06] 解析 URL 查询串
来源：http://bhp.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eok.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dwq.ivvv.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nib.yanxiufei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pjc.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qrb.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qmz.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tgy.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nkh.tian-w.cn

[K07] 进制转换
来源：http://hwi.chenjidiqi.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uyt.0kj1m.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://euf.epnwcf.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jyz.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ami.uphjek.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://the.shanyushiyangtech.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://iri.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://sgv.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://plx.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://cwz.zhongyouzk.top

Py:   pickle.dumps(obj)
来源：http://fld.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wwu.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://chd.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://ikb.cucudq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wpn.yj20258888.top


<!-- 参考信息 -->