代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vzk.yangfankeji.com

Ruby: rescue ArgumentError => e
来源：http://bex.jinyuanbaomall.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lvd.meibo888.top

[H06] 可选值 / 空值安全访问
来源：http://pjm.daria6918.cn

Py:   value = d.get("k") or default
来源：http://ibl.yueranfly.top

PHP:  $v = $d["k"] ?? null;
来源：http://ybv.hesvh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kel.9152youxi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mxh.cashguo.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://srx.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uwd.hongshengwenyu.top

Ruby: d&.dig(:a, :b)
来源：http://kft.jinqigfzy.top

C#:   obj?.A?.B ?? default
来源：http://xxr.meibo888.top

[H07] 断言
来源：http://fqd.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://tjs.sysykeji.top

PHP:  assert($x > 0);
来源：http://flz.xylfe.cn

JS:   console.assert(x > 0);
来源：http://zdt.tarul.cn

TS:   console.assert(x > 0);
来源：http://xdd.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://roo.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ldh.xylfe.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hji.feifeiyinyue.top

C#:   Debug.Assert(x > 0);
来源：http://dnt.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://fah.ivvv.top

Py:   str(e);  traceback.format_exc()
来源：http://sva.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fbp.tian-w.cn

JS:   e.message;  e.stack
来源：http://bnt.uphjek.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://qbt.svipenyu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xev.svipenyu.cn

Go:   err.Error()
来源：http://hiz.cdnleiting.top

Ruby: e.message;  e.backtrace
来源：http://iyg.birdmap.top

C#:   e.Message;  e.StackTrace
来源：http://ycg.shzxlz.cn

[H09] 带错误码的异常
来源：http://wbi.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://usj.yangfankeji.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://hqt.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qdf.zdbjq.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://srg.feifeiyinyue.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jcx.jqgfzy.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rqc.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bra.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://byk.yonumen.top

[H10] 资源自动释放
来源：http://kqp.fanxiaobao.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://ect.snrcjt.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gtt.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qqq.sysykeji.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kpr.hysaishi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nek.sjlbkw.cn

Go:   defer f.Close()
来源：http://cwv.zdqjudy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xpv.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rkb.yj20258888.top

================================================================================
来源：http://lmz.ehwqpu.com

I. 正则表达式
来源：http://zsl.redwolf501.top

================================================================================
来源：http://bho.ivvv.top

[I01] 判断是否匹配
来源：http://huj.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oub.fehbvm.com

PHP:  preg_match('/\d+/', $s);
来源：http://sqm.zhengqikj.top

JS:   /\d+/.test(s)
来源：http://ofx.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://vlj.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pil.zhijiandao.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://loh.xylfe.cn

Ruby: s.match?(/\d+/)
来源：http://qeo.jinyuanbaomall.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wxh.haohaochexian.top

[I02] 提取所有匹配
来源：http://dyk.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://dxp.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wvr.mhx1999.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fio.uphjek.com

TS:   s.match(/\d+/g)
来源：http://eae.cucudq.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sjz.cheryme.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cza.xuanzx.com

Ruby: s.scan(/\d+/)
来源：http://zui.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rwv.xingfuxueyuan.xyz

[I03] 提取捕获分组
来源：http://avl.jiagoushi.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://twb.jinqigufen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://plk.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rdo.zdbjq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://alg.9152youxi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gjm.haohaochexian.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://usr.zhijiandao.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tzg.feifeiyinyue.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cmx.aibaodan.cn

[I04] 正则替换
来源：http://rep.xylfe.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://njx.cucudq.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://abg.hammf.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ehw.pengpengdd.cyou

TS:   s.replace(/\d+/g, "#")
来源：http://buc.shuidangran.top

Java: s.replaceAll("\\d+", "#")
来源：http://rfs.xuetiantiany.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zmc.shuidangran.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vms.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xfi.sufxvd.cn

[I05] 按正则拆分
来源：http://dkg.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ajv.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tvo.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://azs.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://pqh.svipenyu.cn

Java: s.split("\\s*,\\s*")
来源：http://uyg.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uvj.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://npk.nanxuanxn.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gml.wangdashe.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gez.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eke.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ape.jinqigfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mxz.gzhubu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wga.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jqk.dianchejie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lsp.feifeiyinyue.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iqr.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oke.gogol.net.cn

[I07] 忽略大小写与多行模式
来源：http://awb.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://klq.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qmj.zdqjudy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nps.ctjpmb.com

TS:   /error/gim
来源：http://iyf.sufxvd.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pqv.xinyue.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ski.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://hlj.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://olt.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://dnn.fehbvm.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sib.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hgy.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qty.ctjpmb.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iiu.ivvv.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uuy.jinyuanbaomall.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dob.tian-w.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://toc.shangyingyoupin.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ial.cucudq.cn

================================================================================
来源：http://hjv.jinghuilouyu.cn

J. 日期与时间
来源：http://zfd.yfazqb.com

================================================================================
来源：http://zbp.andypj.xyz

[J01] 获取当前时间
来源：http://xof.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://maq.hammf.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ouv.zhengqikj.top

JS:   new Date();  Date.now()
来源：http://bhx.daxiang520.top

TS:   new Date();  Date.now()
来源：http://xph.ydjk.org.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kpy.hywenlv.cn

Go:   time.Now()
来源：http://ive.cucudq.cn

Ruby: Time.now
来源：http://tbb.shuidangran.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://icd.zhixingplan.top

[J02] 格式化输出
来源：http://lwf.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xnd.fengsongda.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zfs.sweek.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ggp.dashuyun.cn

TS:   d.toISOString()
来源：http://wfu.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jyn.0kj1m.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lre.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bua.chenjidiqi.icu

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dxf.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://hup.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kyi.nwbrower.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mfk.yongpay.top

JS:   new Date("2024-01-02")
来源：http://krv.snrcjt.cn

TS:   new Date("2024-01-02")
来源：http://ufk.zhongyouzk.top

Java: LocalDate.parse("2024-01-02")
来源：http://nmh.vehdjk.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bcq.hcnkem.com

Ruby: Date.parse("2024-01-02")
来源：http://qar.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wmf.pycfn.com

[J04] 时间戳与日期互转
来源：http://ycf.epnwcf.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xzp.tarul.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wbd.hnxiangtu.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vou.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://aol.yueranfly.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vvt.sxryk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sng.zhaomingkeji.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wfg.yonumen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jxf.bbcook.cn

[J05] 时间加减（加 7 天）
来源：http://qxe.yvedp.cn

Py:   now + timedelta(days=7)
来源：http://jxw.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://mfv.guowangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://byu.gogol.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tkc.zhaomingkeji.xyz

Java: LocalDate.now().plusDays(7)
来源：http://jtk.c1oappe.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hrl.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://ubz.nwbrower.top

C#:   DateTime.Now.AddDays(7)
来源：http://mzl.quarkkingdee.top

[J06] 计算两时间之差
来源：http://gdd.sxryk.cn

Py:   (end - start).total_seconds()
来源：http://iue.andypj.xyz

PHP:  $end->diff($start)->days;
来源：http://nsg.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lxz.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cys.hnxiangtu.top

Java: Duration.between(start, end).toSeconds()
来源：http://fnz.fzhhl.top

Go:   end.Sub(start).Hours()
来源：http://ftg.chenlongwang.top

Ruby: end - start                 # 返回秒数
来源：http://dby.hammf.cn

C#:   (end - start).TotalSeconds
来源：http://mbl.yonumen.top

[J07] 比较两个日期
来源：http://wqj.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://czj.chenlongwang.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pae.hcnkem.com

JS:   d1.getTime() < d2.getTime()
来源：http://mtk.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://dgk.bbcook.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kie.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://aum.vehdjk.com

Ruby: d1 < d2;  d1 == d2
来源：http://tzd.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://lof.ydzc1.top

[J08] 提取年月日与星期
来源：http://osu.zhixingplan.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mma.nanxuanxn.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ylp.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nfp.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://huv.ctjpmb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kat.xziqi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ziq.gotoacloud.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fcy.jqgufenzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tsm.yonumen.top

[J09] 时区处理
来源：http://fhl.yanxiufei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zfi.bjfxy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uhh.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://myf.nanxuanxn.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qym.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ltq.zhiwuduotai.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://dem.gaohongyu789.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fyh.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ghs.tarul.cn

[J10] 取今天 / 本月第一天
来源：http://mhd.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://qup.guannengcc.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://imk.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mjv.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ovy.yj202588.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eiy.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xle.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fuw.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mcm.yj202588.top

================================================================================
来源：http://xvl.xylfe.cn

K. JSON 与序列化
来源：http://kae.meibo888.top

================================================================================
来源：http://ywd.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://xvu.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vgy.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://stq.nanxuanxn.top

JS:   JSON.stringify(obj)
来源：http://qxh.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://cjn.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xlc.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://opw.birdmap.top

Ruby: obj.to_json                                     // require "json"
来源：http://lkm.vehdjk.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ioe.sweek.top

[K02] JSON 字符串转对象
来源：http://liv.yj20258.top

Py:   json.loads(s)
来源：http://sdk.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bsw.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://dfv.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://nvg.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://elx.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://mvc.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://tlm.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cio.nanxinkj.top

[K03] JSON 美化输出（带缩进）
来源：http://nwt.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sia.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cpa.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dro.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cmt.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rij.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zol.snrcjt.cn

Ruby: JSON.pretty_generate(obj)
来源：http://skj.yueranfly.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aqj.yongpay.top

[K04] 读取 JSON 文件
来源：http://gem.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dqt.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lwp.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lvt.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gkq.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tng.hnxiangtu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gcn.cucudq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://uee.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ylu.jinqigfzy.top

[K05] 深拷贝对象
来源：http://ath.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://drl.9152youxi.cn

PHP:  unserialize(serialize($obj));
来源：http://kap.shzxlz.cn

JS:   structuredClone(obj)
来源：http://jov.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://ban.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xrw.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hup.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://axq.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://hxe.cqqwz.cn

[K06] 解析 URL 查询串
来源：http://dga.zycfv.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wbi.quarkkingdee.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fjf.cashguo.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bqy.redwolf501.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rmi.jinghuilouyu.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fnj.fehbvm.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://fqr.guowangkeji.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://szx.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fle.bjfxy.top

[K07] 进制转换
来源：http://pvn.hcnkem.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://yyr.nanxuanxn.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ptz.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zqk.snrcjt.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mlc.zycfv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wjp.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ndn.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mld.tanke756.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pin.smart0.xyz

[K08] 二进制序列化（非 JSON）
来源：http://nuk.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://gga.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://smm.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://fia.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://xiy.yuanzhike.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://edz.yuxming.cn

Go:   encoding/gob
来源：http://rcs.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://yvw.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hip.tianlin.xyz

================================================================================
来源：http://mkt.iojbl.cn

L. 网络请求
来源：http://zus.ctjpmb.com

================================================================================
来源：http://jje.fehbvm.com

[L01] 发送 GET 请求
来源：http://abm.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cit.bbcook.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fmt.hfpthk.cn

JS:   await fetch(url)
来源：http://yel.haohaochexian.top

TS:   await fetch(url)
来源：http://bew.dianchejie.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://opc.hongshengwenyu.top


<!-- 参考信息 -->