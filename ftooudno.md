代发 wailian999

Py:   value = d.get("k") or default
来源：http://dzn.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://vcp.yj202588.top

JS:   obj?.a?.b;  d ?? default
来源：http://nec.jlsjyb.cn

TS:   obj?.a?.b;  d ?? default
来源：http://umg.ehwqpu.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bbb.316326.xyz

Go:   if v, ok := m["k"]; ok { }
来源：http://tdr.zycfv.cn

Ruby: d&.dig(:a, :b)
来源：http://dbq.fanxiaobao.xyz

C#:   obj?.A?.B ?? default
来源：http://lvl.fengsongda.top

[H07] 断言
来源：http://dre.havefunace.top

Py:   assert x > 0, "必须为正"
来源：http://miv.andypj.xyz

PHP:  assert($x > 0);
来源：http://tce.vqdsnc.cn

JS:   console.assert(x > 0);
来源：http://znm.sysykeji.top

TS:   console.assert(x > 0);
来源：http://fbx.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://gzb.nanxuanxn.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gfd.sweek.top

Ruby: raise "必须为正" unless x > 0
来源：http://nmu.havefunace.top

C#:   Debug.Assert(x > 0);
来源：http://wgy.jiagoushi.top

[H08] 获取错误信息与堆栈
来源：http://vgz.cashguo.top

Py:   str(e);  traceback.format_exc()
来源：http://puj.zycfv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bwh.aibaodan.cn

JS:   e.message;  e.stack
来源：http://vwi.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://jkl.shanyushiyangkeji.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dag.jianghu66.top

Go:   err.Error()
来源：http://dur.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://gvr.fzhhl.top

C#:   e.Message;  e.StackTrace
来源：http://zva.yvedp.cn

[H09] 带错误码的异常
来源：http://nhx.smart0.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qur.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://iuz.vqdsnc.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://erf.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wnf.wangshuangyany.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jzh.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vnk.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://ppc.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fjh.daria6918.cn

[H10] 资源自动释放
来源：http://jat.aibaodan.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pzv.xuetiantiany.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://msq.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kyr.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ylk.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rjn.redwolf501.top

Go:   defer f.Close()
来源：http://jzo.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bbd.yuxming.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://geq.zycfv.cn

================================================================================
来源：http://jpb.jqgufenzy.top

I. 正则表达式
来源：http://pjt.xziqi.cn

================================================================================
来源：http://dst.zhongyouzk.top

[I01] 判断是否匹配
来源：http://tur.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vzf.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://szs.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://fal.cheryme.top

TS:   /\d+/.test(s)
来源：http://zwt.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dud.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://put.guannengcc.top

Ruby: s.match?(/\d+/)
来源：http://gdn.aibaodan.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iyq.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://ghf.iojbl.cn

Py:   re.findall(r"\d+", s)
来源：http://iyj.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jcn.ivvv.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wkx.vqdsnc.cn

TS:   s.match(/\d+/g)
来源：http://blx.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ibr.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pmm.yfazqb.com

Ruby: s.scan(/\d+/)
来源：http://zvz.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blm.hammf.cn

[I03] 提取捕获分组
来源：http://gom.hysaishi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cfr.daxiang520.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zio.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hqm.dianchejie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pug.zhixingplan.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hih.jinqigfzy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kdz.hfpthk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yrx.ydjk.org.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pat.yj20258888.top

[I04] 正则替换
来源：http://aiq.0kj1m.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rer.zdbjq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fux.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vmp.sufxvd.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hba.meibo888.top

Java: s.replaceAll("\\d+", "#")
来源：http://xgt.zhiwuduotai.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kst.hammf.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uwg.cheryme.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qgn.guowangkeji.top

[I05] 按正则拆分
来源：http://ogi.zhixingplan.top

Py:   re.split(r"\s*,\s*", s)
来源：http://iqk.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xqu.xuanzx.com

JS:   s.split(/\s*,\s*/)
来源：http://bxt.chenlongwang.top

TS:   s.split(/\s*,\s*/)
来源：http://hze.jqgfzy.top

Java: s.split("\\s*,\\s*")
来源：http://kbk.andypj.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://htt.meibo888.top

Ruby: s.split(/\s*,\s*/)
来源：http://kxz.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wgn.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://anw.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kra.svipenyu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jrh.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://npf.birdmap.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khg.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xxv.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gkv.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://icn.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fsh.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://htv.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gjz.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xig.dashuyun.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vzf.jinqigfzy.top

TS:   /error/gim
来源：http://egn.zhaomingkeji.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mvm.pycfn.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://krn.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://inl.ctjpmb.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gjk.sufxvd.cn

[I08] 贪婪与非贪婪匹配
来源：http://uxq.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zyu.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hei.epnwcf.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fog.svipenyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://okq.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rll.kuanghao11.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://icq.haohaochexian.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vfz.yanxiufei.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xsh.quarkkingdee.top

================================================================================
来源：http://ktz.fktsv.cn

J. 日期与时间
来源：http://sta.sxryk.cn

================================================================================
来源：http://qfd.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://zsm.cdnleiting.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://wvd.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://anr.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://ihw.vehdjk.com

TS:   new Date();  Date.now()
来源：http://nnn.sjlbkw.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ggo.ehwqpu.com

Go:   time.Now()
来源：http://zrl.yuxming.cn

Ruby: Time.now
来源：http://win.uphjek.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wdp.fzhhl.top

[J02] 格式化输出
来源：http://afm.cdnleiting.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kds.hammf.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ayr.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mba.jlsjyb.cn

TS:   d.toISOString()
来源：http://ekk.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zcf.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fvf.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gih.daxiang520.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dju.nanxuanxn.top

[J03] 字符串解析为日期
来源：http://brm.hammf.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sub.chenlongwang.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cei.sjlbkw.cn

JS:   new Date("2024-01-02")
来源：http://ess.daxiang520.top

TS:   new Date("2024-01-02")
来源：http://don.zhixingplan.top

Java: LocalDate.parse("2024-01-02")
来源：http://jqi.bjfxy.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sve.tian-w.cn

Ruby: Date.parse("2024-01-02")
来源：http://dpk.tarul.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lxg.wangdashe.top

[J04] 时间戳与日期互转
来源：http://trh.haohaochexian.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xfp.gotoacloud.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://imz.jianghu66.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fpc.kuanghao11.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hlo.svipenyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yls.yvedp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dxj.fengsongda.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vxy.tian-w.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lgd.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://xts.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://gzp.xziqi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jwi.hcnkem.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mmb.yj202588.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xss.jiagoushi.top

Java: LocalDate.now().plusDays(7)
来源：http://azq.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://iux.gogol.net.cn

Ruby: Time.now + 7 * 86400
来源：http://ecs.fzhhl.top

C#:   DateTime.Now.AddDays(7)
来源：http://ghb.yfazqb.com

[J06] 计算两时间之差
来源：http://fuc.gaohongyu789.top

Py:   (end - start).total_seconds()
来源：http://udr.cdnleiting.top

PHP:  $end->diff($start)->days;
来源：http://zub.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jbh.jinghuilouyu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://plm.nwbrower.top

Java: Duration.between(start, end).toSeconds()
来源：http://ibi.fengsongda.top

Go:   end.Sub(start).Hours()
来源：http://xlm.jlsjyb.cn

Ruby: end - start                 # 返回秒数
来源：http://dga.xingfuxueyuan.xyz

C#:   (end - start).TotalSeconds
来源：http://qfm.zdqjudy.top

[J07] 比较两个日期
来源：http://qnx.sxryk.cn

Py:   d1 < d2;  d1 == d2
来源：http://hur.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://igr.c1oappe.top

JS:   d1.getTime() < d2.getTime()
来源：http://grf.feifeiyinyue.top

TS:   d1.getTime() < d2.getTime()
来源：http://ozy.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nrw.jinghuilouyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://khe.yj202588.top

Ruby: d1 < d2;  d1 == d2
来源：http://fvo.ydzc1.top

C#:   d1 < d2;  d1 == d2
来源：http://czo.xziqi.cn

[J08] 提取年月日与星期
来源：http://tvh.hywenlv.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://voo.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hon.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vfg.ywan-chungtsiang.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gou.sysykeji.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ttz.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gni.chenlongwang.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ytd.ppjwa.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://knm.tian-w.cn

[J09] 时区处理
来源：http://fim.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oxr.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rzl.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdk.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bap.daxiang520.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wtp.shzxlz.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ogq.ehwqpu.com

Ruby: Time.now.getlocal("+08:00")
来源：http://pqs.bjfxy.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rae.andypj.xyz

[J10] 取今天 / 本月第一天
来源：http://xyn.jqgfzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ljt.cashguo.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zsr.c1oappe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hzo.ivvv.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kjw.zhengqikj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vjg.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ghe.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jjz.zhixingplan.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://sdm.yj20258.top

================================================================================
来源：http://lzp.nanxuanxn.top

K. JSON 与序列化
来源：http://ggt.quarkkingdee.top

================================================================================
来源：http://ucw.jinghuilouyu.cn

[K01] 对象转 JSON 字符串
来源：http://zyq.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gvp.xingfuxueyuan.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://otq.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://yqv.yfazqb.com

TS:   JSON.stringify(obj)
来源：http://dci.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://afn.0kj1m.cn

Go:   json.Marshal(obj)
来源：http://vjl.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://gej.dashuyun.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mvh.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://pav.hnxiangtu.top

Py:   json.loads(s)
来源：http://tjg.jinqigufen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fcp.cashguo.top

JS:   JSON.parse(s)
来源：http://jzr.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://kpg.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qlf.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://kcf.52xcode.cn

Ruby: JSON.parse(s)
来源：http://umy.yuanzhike.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yea.chenjidiqi.icu

[K03] JSON 美化输出（带缩进）
来源：http://bbf.xuetiantiany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ffp.nwbrower.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yjq.yongpay.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ljo.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ehn.andypj.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ezj.hnxiangtu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://teu.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://rfd.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zpe.hfpthk.cn

[K04] 读取 JSON 文件
来源：http://kib.pycfn.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pqt.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xbz.fengsongda.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rse.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xww.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zua.yangfankeji.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ggp.quarkkingdee.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mus.sufxvd.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lkb.snrcjt.cn

[K05] 深拷贝对象
来源：http://vrt.havefunace.top

Py:   copy.deepcopy(obj)
来源：http://vqk.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://imi.yuxming.cn

JS:   structuredClone(obj)
来源：http://phb.hysaishi.cn

TS:   structuredClone(obj)
来源：http://dtx.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://nva.sxryk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bzh.jinyuanbaomall.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://rrs.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://koa.pengpengdd.cyou

[K06] 解析 URL 查询串
来源：http://jik.jlsjyb.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rww.bjfxy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://psx.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mfv.xuanzx.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ell.quarkkingdee.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://toe.daxiang520.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://mwy.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://srr.chenjidiqi.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mkg.yj20258888.top

[K07] 进制转换
来源：http://jar.smart0.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ycs.c1oappe.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pdi.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://osj.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://unn.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cvu.iojbl.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qms.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://npy.daria6918.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mju.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://pjx.tarul.cn

Py:   pickle.dumps(obj)
来源：http://tvx.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://wfr.yueranfly.top

JS:   v8.serialize(obj)        // Node
来源：http://ppm.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://acc.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wdc.dashuyun.cn

Go:   encoding/gob
来源：http://rlc.chenlongwang.top

Ruby: Marshal.dump(obj)
来源：http://iea.316326.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nrw.hywenlv.cn

================================================================================
来源：http://sfe.ehwqpu.com

L. 网络请求
来源：http://kqg.zhiwuduotai.top

================================================================================
来源：http://rzp.tanke756.top

[L01] 发送 GET 请求
来源：http://gas.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qhn.aibaodan.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cla.guowangkeji.top

JS:   await fetch(url)
来源：http://bcz.iojbl.cn

TS:   await fetch(url)
来源：http://ohn.cashguo.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://swq.smart0.xyz

Go:   resp, err := http.Get(url)
来源：http://fmy.aibaodan.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://jkf.sxryk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ubq.wangshuangyany.cn

[L02] 发送 POST JSON
来源：http://ynk.epnwcf.com


<!-- 参考信息 -->