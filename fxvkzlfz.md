代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oxs.fktsv.cn

JS:   if (e instanceof TypeError) {}
来源：http://nry.smart0.xyz

TS:   if (e instanceof TypeError) {}
来源：http://psc.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://raj.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eqx.fehbvm.com

Ruby: rescue ArgumentError => e
来源：http://lsi.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://khz.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://yfr.hcnkem.com

Py:   value = d.get("k") or default
来源：http://zsl.dashuyun.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tjr.xziqi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jrf.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://crb.zhoulong.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qai.jlsjyb.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ulc.wangdashe.top

Ruby: d&.dig(:a, :b)
来源：http://vzj.redwolf501.top

C#:   obj?.A?.B ?? default
来源：http://xyb.xinyue.icu

[H07] 断言
来源：http://abp.tarul.cn

Py:   assert x > 0, "必须为正"
来源：http://uvq.shangyingyoupin.top

PHP:  assert($x > 0);
来源：http://tzb.zhijiandao.cn

JS:   console.assert(x > 0);
来源：http://eln.xinyue.icu

TS:   console.assert(x > 0);
来源：http://etg.zhengqikj.top

Java: assert x > 0 : "必须为正";
来源：http://zwv.gzhubu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fhm.cashguo.top

Ruby: raise "必须为正" unless x > 0
来源：http://vui.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://kee.yj20258.top

[H08] 获取错误信息与堆栈
来源：http://fsp.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://emm.jinghuilouyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ucy.52xcode.cn

JS:   e.message;  e.stack
来源：http://mpi.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://evc.yueranfly.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wmg.hongshengwenyu.top

Go:   err.Error()
来源：http://rgc.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://epi.xingfuxueyuan.xyz

C#:   e.Message;  e.StackTrace
来源：http://zyp.wangshuangyany.cn

[H09] 带错误码的异常
来源：http://nvc.xinyue.icu

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tvn.hongshengwenyu.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bzd.yj20258.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zan.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ctu.hammf.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cdt.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yxf.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://uzm.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fvs.yuxming.cn

[H10] 资源自动释放
来源：http://vkn.guannengcc.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://qoo.meibo888.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uup.hcnkem.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dyv.dashuyun.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jmo.jiagoushi.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bku.fehbvm.com

Go:   defer f.Close()
来源：http://dnu.guowangkeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bwb.iojbl.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uaq.daxiang520.top

================================================================================
来源：http://vkv.shanyushiyangtech.top

I. 正则表达式
来源：http://pcs.jinqigfzy.top

================================================================================
来源：http://msy.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://nvv.yangfankeji.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://enw.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rhe.yj20258.top

JS:   /\d+/.test(s)
来源：http://fgg.ivvv.top

TS:   /\d+/.test(s)
来源：http://wxa.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tsv.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vwq.shanyushiyangtech.top

Ruby: s.match?(/\d+/)
来源：http://mjm.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blz.xingfuxueyuan.xyz

[I02] 提取所有匹配
来源：http://nki.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://hnd.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtb.havefunace.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gzu.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://khu.ctjpmb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rur.cdnleiting.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wxn.snrcjt.cn

Ruby: s.scan(/\d+/)
来源：http://afq.nanxinkj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ffb.yuanzhike.top

[I03] 提取捕获分组
来源：http://iao.guowangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jyb.yongpay.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ccs.tianlin.xyz

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hcn.ybcxt.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yrz.quarkkingdee.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fmr.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wbo.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aiv.shanyushiyangkeji.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://urt.zhijiandao.cn

[I04] 正则替换
来源：http://jtz.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bln.nanxinkj.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pnf.316326.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://lpz.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://xaq.hesvh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fbs.tanke756.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qwe.jiagoushi.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pzv.ybcxt.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wun.cqqwz.cn

[I05] 按正则拆分
来源：http://ycj.quarkkingdee.top

Py:   re.split(r"\s*,\s*", s)
来源：http://vhd.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qru.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://doe.yonumen.top

TS:   s.split(/\s*,\s*/)
来源：http://ldp.fanxiaobao.xyz

Java: s.split("\\s*,\\s*")
来源：http://kof.yj20258.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wmb.chenjidiqi.icu

Ruby: s.split(/\s*,\s*/)
来源：http://ita.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rin.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kbs.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nnd.cucudq.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://plw.ppjwa.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xoa.tianlin.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uni.9152youxi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dhr.sxryk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wrk.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://znk.zhixingplan.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mbg.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://gtv.yfazqb.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xxi.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mov.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yvs.cashguo.top

TS:   /error/gim
来源：http://kym.hongshengwenyu.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xis.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mhd.cashguo.top

Ruby: s.scan(/error/i)
来源：http://tpu.hammf.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zmq.ivvv.top

[I08] 贪婪与非贪婪匹配
来源：http://xxw.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iql.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uvd.nanxuanxn.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ybi.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hdv.yfazqb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://tgq.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dfm.vehdjk.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ksk.fktsv.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hxo.dashuyun.cn

================================================================================
来源：http://vml.vqdsnc.cn

J. 日期与时间
来源：http://win.yangfankeji.com

================================================================================
来源：http://gyx.mhx1999.top

[J01] 获取当前时间
来源：http://ggv.9152youxi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://erx.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ivh.zycfv.cn

JS:   new Date();  Date.now()
来源：http://nsc.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://gvr.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gjn.zhijiandao.cn

Go:   time.Now()
来源：http://nta.hesvh.cn

Ruby: Time.now
来源：http://ogq.jyoumei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://slf.andypj.xyz

[J02] 格式化输出
来源：http://wch.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://clx.birdmap.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wqg.shangyingyoupin.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aii.cheryme.top

TS:   d.toISOString()
来源：http://lxc.dianchejie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://itr.tarul.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ywr.gaohongyu789.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxt.jinqigufen.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://esj.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://nef.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bxq.iojbl.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qlr.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://akz.zycfv.cn

TS:   new Date("2024-01-02")
来源：http://sec.xinyue.icu

Java: LocalDate.parse("2024-01-02")
来源：http://lpg.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vrp.jyoumei.cn

Ruby: Date.parse("2024-01-02")
来源：http://cgt.pycfn.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jmm.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://wli.zdbjq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rta.yfazqb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fba.0kj1m.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nyv.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gcm.zhoulong.xyz

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qjc.nanxinkj.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://omi.sjlbkw.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://unb.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qzt.xingfuxueyuan.xyz

[J05] 时间加减（加 7 天）
来源：http://xsz.hesvh.cn

Py:   now + timedelta(days=7)
来源：http://ngj.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://cep.feifeiyinyue.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhx.nanxuanxn.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qmt.aibaodan.cn

Java: LocalDate.now().plusDays(7)
来源：http://fcx.xuetiantiany.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://byb.hammf.cn

Ruby: Time.now + 7 * 86400
来源：http://bld.bjfxy.top

C#:   DateTime.Now.AddDays(7)
来源：http://nus.cucudq.cn

[J06] 计算两时间之差
来源：http://oyf.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://mrp.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://vrx.cashguo.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tbp.hammf.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gcu.jinyuanbaomall.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qft.guowangkeji.top

Go:   end.Sub(start).Hours()
来源：http://zeb.jinyuanbaomall.cn

Ruby: end - start                 # 返回秒数
来源：http://wxk.cashguo.top

C#:   (end - start).TotalSeconds
来源：http://jvu.birdmap.top

[J07] 比较两个日期
来源：http://rgu.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://knr.haohaochexian.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kwd.zhiwuduotai.top

JS:   d1.getTime() < d2.getTime()
来源：http://wix.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://abt.ybcxt.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fdw.dashuyun.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sin.ydjk.org.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yft.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://czi.chenzaomai.com

[J08] 提取年月日与星期
来源：http://wkg.nanxinkj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bxu.vehdjk.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://sbo.tarul.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://oga.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zod.smart0.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jwy.ywan-chungtsiang.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pbu.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vbk.cashguo.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://skf.hesvh.cn

[J09] 时区处理
来源：http://nnv.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rus.0kj1m.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://kwh.hysaishi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vyr.chenzaomai.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zsm.jqgfzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hkn.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aqg.fengsongda.top

Ruby: Time.now.getlocal("+08:00")
来源：http://txs.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qgl.pengpengdd.cyou

[J10] 取今天 / 本月第一天
来源：http://dnj.uphjek.com

Py:   date.today();  date.today().replace(day=1)
来源：http://xgr.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jtk.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vuh.sjlbkw.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cbs.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qqo.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jef.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lcc.jqgufenzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jat.zdqjudy.top

================================================================================
来源：http://ror.tianlin.xyz

K. JSON 与序列化
来源：http://glm.nwbrower.top

================================================================================
来源：http://ajr.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://heg.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://knj.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wni.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://fuv.tarul.cn

TS:   JSON.stringify(obj)
来源：http://bch.redwolf501.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://meo.jqgufenzy.top

Go:   json.Marshal(obj)
来源：http://zaf.tianlin.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://kqz.hnxiangtu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hlz.jianghu66.top

[K02] JSON 字符串转对象
来源：http://obv.jinqigfzy.top

Py:   json.loads(s)
来源：http://zlp.daria6918.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lgb.gzhubu.top

JS:   JSON.parse(s)
来源：http://uvj.daria6918.cn

TS:   JSON.parse(s)
来源：http://ymh.guowangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xrg.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://jda.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://val.shuidangran.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rvb.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://qil.bbcook.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://imd.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dlt.zhijiandao.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qqw.shuidangran.top

TS:   JSON.stringify(obj, null, 2)
来源：http://xlz.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://scp.sysykeji.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://llc.hammf.cn

Ruby: JSON.pretty_generate(obj)
来源：http://wxy.wangdashe.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iiu.yj20258.top

[K04] 读取 JSON 文件
来源：http://oyq.yj202588.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://huv.ydjk.org.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bey.vqdsnc.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mcz.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cse.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cua.nanxuanxn.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://boh.snrcjt.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://jlg.shanyushiyangkeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fwm.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://jfr.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://nyn.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://wmb.cheryme.top

JS:   structuredClone(obj)
来源：http://ptz.cheryme.top

TS:   structuredClone(obj)
来源：http://rjb.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jvm.yj20258888.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vzk.wangdashe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://opc.shuidangran.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cdb.daxiang520.top

[K06] 解析 URL 查询串
来源：http://fdp.haohaochexian.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jzz.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xds.zhaomingkeji.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ykv.tarul.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gfy.hongshengwenyu.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uzn.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://luz.cdnleiting.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mvm.sufxvd.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ulg.cheryme.top

[K07] 进制转换
来源：http://vns.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sml.yj20258888.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://npn.zhengqikj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pla.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ftc.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oiu.hnqzz.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://czk.gaohongyu789.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oer.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kfi.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://iiq.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://frb.hysaishi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://eni.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://jju.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://kjy.yuxming.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fqo.gogol.net.cn

Go:   encoding/gob
来源：http://psq.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://ipg.0kj1m.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dpq.ydzc1.top

================================================================================
来源：http://lrc.jyoumei.cn

L. 网络请求
来源：http://dbx.c1oappe.top

================================================================================
来源：http://mjx.c1oappe.top

[L01] 发送 GET 请求
来源：http://lga.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ztj.yanxiufei.cn


<!-- 参考信息 -->