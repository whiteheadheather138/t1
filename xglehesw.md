代发 wailian999

Py:   value = d.get("k") or default
来源：http://pyb.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tow.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://ywi.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bcx.zhijiandao.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://djt.hnxiangtu.top

Go:   if v, ok := m["k"]; ok { }
来源：http://apa.yj202588.top

Ruby: d&.dig(:a, :b)
来源：http://pha.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://rct.svipenyu.cn

[H07] 断言
来源：http://gpp.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://prk.fzhhl.top

PHP:  assert($x > 0);
来源：http://emf.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://sie.daxiang520.top

TS:   console.assert(x > 0);
来源：http://mih.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://nkv.zhiwuduotai.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fkm.ybcxt.top

Ruby: raise "必须为正" unless x > 0
来源：http://fsu.pengpengdd.cyou

C#:   Debug.Assert(x > 0);
来源：http://fkb.cheryme.top

[H08] 获取错误信息与堆栈
来源：http://axz.sysykeji.top

Py:   str(e);  traceback.format_exc()
来源：http://bkm.fehbvm.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jik.quarkkingdee.top

JS:   e.message;  e.stack
来源：http://rbx.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://klz.gzhubu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://cou.hywenlv.cn

Go:   err.Error()
来源：http://wqo.sufxvd.cn

Ruby: e.message;  e.backtrace
来源：http://ymg.zhoulong.xyz

C#:   e.Message;  e.StackTrace
来源：http://sls.yanxiufei.cn

[H09] 带错误码的异常
来源：http://pok.havefunace.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hqb.feifeiyinyue.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://tqm.ydjk.org.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vrd.sysykeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jpu.tanke756.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qbk.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hyr.birdmap.top

Ruby: raise MyError.new("fail", 500)
来源：http://sfj.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ilr.shzxlz.cn

[H10] 资源自动释放
来源：http://thq.meibo888.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://kwz.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cwa.xziqi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qsj.fktsv.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qxg.iojbl.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ykz.xinyue.icu

Go:   defer f.Close()
来源：http://vnl.chenjidiqi.icu

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lxc.xingfuxueyuan.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yua.fanxiaobao.xyz

================================================================================
来源：http://cqw.zdbjq.cn

I. 正则表达式
来源：http://psx.wangdashe.top

================================================================================
来源：http://ahn.ivvv.top

[I01] 判断是否匹配
来源：http://xcf.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://elu.hywenlv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nok.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://ouu.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://fyr.hnqzz.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nhz.shanyushiyangkeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xyt.epnwcf.com

Ruby: s.match?(/\d+/)
来源：http://hsi.gogol.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rdq.quarkkingdee.top

[I02] 提取所有匹配
来源：http://csw.yuanzhike.top

Py:   re.findall(r"\d+", s)
来源：http://ruc.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zhg.gzhubu.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gto.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://ihd.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://utq.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vzx.jlsjyb.cn

Ruby: s.scan(/\d+/)
来源：http://wyr.sufxvd.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bof.gaohongyu789.top

[I03] 提取捕获分组
来源：http://ddw.uphjek.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://abp.daria6918.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ymh.zhongyouzk.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kqb.zhijiandao.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lvg.yanxiufei.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vcp.tianlin.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bho.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ekb.sjlbkw.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://chf.chenzaomai.com

[I04] 正则替换
来源：http://tau.shanyushiyangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vsm.zhixingplan.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://obc.cdnleiting.top

JS:   s.replace(/\d+/g, "#")
来源：http://fuf.yvedp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://acf.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qhi.vehdjk.com

Go:   re.ReplaceAllString(s, "#")
来源：http://flw.dianchejie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jao.fzhhl.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mft.xinyue.icu

[I05] 按正则拆分
来源：http://vki.shzxlz.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qiq.shanyushiyangtech.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fov.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://xqt.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://adm.jinqigfzy.top

Java: s.split("\\s*,\\s*")
来源：http://myz.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lpt.shuidangran.top

Ruby: s.split(/\s*,\s*/)
来源：http://mzm.wangshuangyany.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dcb.svipenyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gqd.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdv.yonumen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://itb.gzhubu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oas.chenjidiqi.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iqy.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://afn.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://irq.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rtp.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uyf.dianchejie.cn

[I07] 忽略大小写与多行模式
来源：http://uxa.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://exy.vqdsnc.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fzs.vqdsnc.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lpc.cdnleiting.top

TS:   /error/gim
来源：http://cra.gaohongyu789.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jei.hesvh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qot.kuanghao11.cn

Ruby: s.scan(/error/i)
来源：http://qjn.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ldk.snrcjt.cn

[I08] 贪婪与非贪婪匹配
来源：http://fxj.tarul.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vxv.fzhhl.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zvj.meibo888.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dtl.gogol.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://euq.bbcook.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bly.xuetiantiany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baw.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jvw.uphjek.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://quf.52xcode.cn

================================================================================
来源：http://gbb.kuanghao11.cn

J. 日期与时间
来源：http://ejr.fanxiaobao.xyz

================================================================================
来源：http://nmn.shangyingyoupin.top

[J01] 获取当前时间
来源：http://fgq.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hno.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://voy.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://huw.redwolf501.top

TS:   new Date();  Date.now()
来源：http://qzz.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rux.aizwys.cn

Go:   time.Now()
来源：http://efz.chenlongwang.top

Ruby: Time.now
来源：http://kvy.daria6918.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xax.yanxiufei.cn

[J02] 格式化输出
来源：http://eep.andypj.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ttk.yj20258.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nyk.xziqi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zux.gaohongyu789.top

TS:   d.toISOString()
来源：http://bnf.yangfankeji.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dze.hammf.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ngp.uphjek.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://huk.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rsl.jqgfzy.top

[J03] 字符串解析为日期
来源：http://qej.c1oappe.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vis.hywenlv.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wir.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://hur.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://tse.epnwcf.com

Java: LocalDate.parse("2024-01-02")
来源：http://vid.ybcxt.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lza.zhixingplan.top

Ruby: Date.parse("2024-01-02")
来源：http://pdv.ywan-chungtsiang.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qar.jianghu66.top

[J04] 时间戳与日期互转
来源：http://abe.nwbrower.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cwl.xuetiantiany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://htk.ctjpmb.com

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://utk.pycfn.com

TS:   Math.floor(Date.now() / 1000)
来源：http://xwn.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://uyy.cqqwz.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zkr.jianghu66.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://miw.aibaodan.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zdi.hesvh.cn

[J05] 时间加减（加 7 天）
来源：http://ehl.xuanzx.com

Py:   now + timedelta(days=7)
来源：http://swv.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://aot.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pfa.yongpay.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://clg.zdqjudy.top

Java: LocalDate.now().plusDays(7)
来源：http://bmu.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uif.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://pyb.jianghu66.top

C#:   DateTime.Now.AddDays(7)
来源：http://gyi.fktsv.cn

[J06] 计算两时间之差
来源：http://suf.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://ctl.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://tps.vehdjk.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://myf.chenzaomai.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://spa.316326.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://tnn.meibo888.top

Go:   end.Sub(start).Hours()
来源：http://vas.zhongyouzk.top

Ruby: end - start                 # 返回秒数
来源：http://wcb.chenlongwang.top

C#:   (end - start).TotalSeconds
来源：http://dtz.ehwqpu.com

[J07] 比较两个日期
来源：http://yzn.ybcxt.top

Py:   d1 < d2;  d1 == d2
来源：http://dbw.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://zli.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://oir.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://adg.xziqi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vyp.nanxuanxn.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uzr.jinqigufen.top

Ruby: d1 < d2;  d1 == d2
来源：http://ufa.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://rhf.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://tsy.iojbl.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pid.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gqf.xinyue.icu

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oii.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zdu.zhixingplan.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://paj.pengpengdd.cyou

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kll.tanke756.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ujd.c1oappe.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zdw.cdnleiting.top

[J09] 时区处理
来源：http://hrn.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jbr.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://smw.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yfz.hnqzz.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lhf.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lqm.vehdjk.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vqr.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://qeg.dashuyun.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lkm.guowangkeji.top

[J10] 取今天 / 本月第一天
来源：http://bzw.jinghuilouyu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ztm.jqgfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pfb.haohaochexian.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://otn.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://foz.xuanzx.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xfu.uphjek.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ciu.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pmg.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tpa.gaohongyu789.top

================================================================================
来源：http://pvv.vehdjk.com

K. JSON 与序列化
来源：http://qyc.jinqigufen.top

================================================================================
来源：http://qky.jqgufenzy.top

[K01] 对象转 JSON 字符串
来源：http://ptm.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fin.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kao.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://cma.nanxuanxn.top

TS:   JSON.stringify(obj)
来源：http://imr.hnxiangtu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qzf.xziqi.cn

Go:   json.Marshal(obj)
来源：http://lxs.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://izs.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://yau.aibaodan.cn

[K02] JSON 字符串转对象
来源：http://yhy.smart0.xyz

Py:   json.loads(s)
来源：http://xsv.yangfankeji.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fez.nanxinkj.top

JS:   JSON.parse(s)
来源：http://ujf.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://qdk.shuidangran.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kdl.xuanzx.com

Go:   json.Unmarshal(data, &v)
来源：http://mwy.redwolf501.top

Ruby: JSON.parse(s)
来源：http://ali.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://glm.bjfxy.top

[K03] JSON 美化输出（带缩进）
来源：http://mpa.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eef.hnxiangtu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rtn.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rle.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ezw.yangfankeji.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lat.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jvy.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nyk.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nvq.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://mgh.jiagoushi.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xrl.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mub.cucudq.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hjd.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lwq.quarkkingdee.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cjf.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hys.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://iql.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bnk.jqgufenzy.top

[K05] 深拷贝对象
来源：http://aml.sjlbkw.cn

Py:   copy.deepcopy(obj)
来源：http://rqw.daxiang520.top

PHP:  unserialize(serialize($obj));
来源：http://yga.snrcjt.cn

JS:   structuredClone(obj)
来源：http://ksx.shuidangran.top

TS:   structuredClone(obj)
来源：http://zin.tianlin.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://wbo.yongpay.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hkc.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ret.aizwys.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://rws.yvedp.cn

[K06] 解析 URL 查询串
来源：http://trt.tianlin.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://sgn.52xcode.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vjg.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kih.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://joo.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ftc.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bjf.jlsjyb.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cwa.guowangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wcl.shanyushiyangkeji.top

[K07] 进制转换
来源：http://nxb.xuetiantiany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uko.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hzz.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yss.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zzv.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kgt.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tru.gogol.net.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://drd.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gcm.zhengqikj.top

[K08] 二进制序列化（非 JSON）
来源：http://vtn.jyoumei.cn

Py:   pickle.dumps(obj)
来源：http://spp.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zfw.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://asy.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://blt.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://owr.xylfe.cn

Go:   encoding/gob
来源：http://txs.yj202588.top

Ruby: Marshal.dump(obj)
来源：http://lsr.sjlbkw.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kxm.shuidangran.top

================================================================================
来源：http://iqd.wangdashe.top

L. 网络请求
来源：http://byp.yuxming.cn

================================================================================
来源：http://gyj.tianlin.xyz

[L01] 发送 GET 请求
来源：http://dcf.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rwr.andypj.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wps.bjfxy.top

JS:   await fetch(url)
来源：http://uzv.meibo888.top

TS:   await fetch(url)
来源：http://jrg.feifeiyinyue.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qdo.pycfn.com

Go:   resp, err := http.Get(url)
来源：http://kuh.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vfg.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uje.nanxuanxn.top

[L02] 发送 POST JSON
来源：http://gxn.chenzaomai.com


<!-- 参考信息 -->