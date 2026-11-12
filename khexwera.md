代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ggw.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://zny.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://ntb.ivvv.top

Java: catch (IOException | SQLException e) {}
来源：http://nxu.meibo888.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cnk.yj20258.top

Ruby: rescue ArgumentError => e
来源：http://ypv.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nej.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://zmf.ivvv.top

Py:   value = d.get("k") or default
来源：http://cui.yanxiufei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://erj.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://qlp.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://kgw.xingfuxueyuan.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://osq.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://dqk.zhongyouzk.top

Ruby: d&.dig(:a, :b)
来源：http://hfk.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://ljm.jinqigfzy.top

[H07] 断言
来源：http://zgx.feifeiyinyue.top

Py:   assert x > 0, "必须为正"
来源：http://twi.hnqzz.top

PHP:  assert($x > 0);
来源：http://kin.yj20258888.top

JS:   console.assert(x > 0);
来源：http://wfq.9152youxi.cn

TS:   console.assert(x > 0);
来源：http://sgy.tianlin.xyz

Java: assert x > 0 : "必须为正";
来源：http://kmr.ybcxt.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lgj.gotoacloud.top

Ruby: raise "必须为正" unless x > 0
来源：http://dtq.mhx1999.top

C#:   Debug.Assert(x > 0);
来源：http://cjz.nwbrower.top

[H08] 获取错误信息与堆栈
来源：http://ewm.xziqi.cn

Py:   str(e);  traceback.format_exc()
来源：http://itt.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xih.yvedp.cn

JS:   e.message;  e.stack
来源：http://sie.hnqzz.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://gdn.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://lvs.ppjwa.cn

Go:   err.Error()
来源：http://ehj.shanyushiyangtech.top

Ruby: e.message;  e.backtrace
来源：http://lez.sufxvd.cn

C#:   e.Message;  e.StackTrace
来源：http://hni.nanxinkj.top

[H09] 带错误码的异常
来源：http://uav.epnwcf.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yuo.kuanghao11.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwj.yj20258888.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qko.hnxiangtu.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cyd.yueranfly.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oxl.cheryme.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ysc.jinqigufen.top

Ruby: raise MyError.new("fail", 500)
来源：http://plj.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rew.kuanghao11.cn

[H10] 资源自动释放
来源：http://pcd.fengsongda.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ygm.hnxiangtu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sfq.cdnleiting.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rfl.sufxvd.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gpo.yfazqb.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fia.hnqzz.top

Go:   defer f.Close()
来源：http://sus.jianghu66.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yzb.jqgfzy.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cce.dianchejie.cn

================================================================================
来源：http://uox.ctjpmb.com

I. 正则表达式
来源：http://vzb.zhengqikj.top

================================================================================
来源：http://rch.0kj1m.cn

[I01] 判断是否匹配
来源：http://rsz.vqdsnc.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://efp.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://vyk.ydjk.org.cn

JS:   /\d+/.test(s)
来源：http://zdj.yuanzhike.top

TS:   /\d+/.test(s)
来源：http://jax.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xaq.fktsv.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mio.fktsv.cn

Ruby: s.match?(/\d+/)
来源：http://znq.birdmap.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mgr.meibo888.top

[I02] 提取所有匹配
来源：http://cpd.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://ciq.aizwys.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dsp.andypj.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://udb.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://gdg.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nru.pycfn.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://skr.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://bcc.xuetiantiany.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wpn.cqqwz.cn

[I03] 提取捕获分组
来源：http://bmv.yangfankeji.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xrk.gzhubu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://iwj.hcnkem.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dpp.jinqigfzy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nxf.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ahu.shanyushiyangtech.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pvk.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dnp.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uxv.shanyushiyangkeji.top

[I04] 正则替换
来源：http://usp.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ijk.yonumen.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nbp.svipenyu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wyr.bbcook.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yga.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uke.sweek.top

Go:   re.ReplaceAllString(s, "#")
来源：http://bqb.havefunace.top

Ruby: s.gsub(/\d+/, "#")
来源：http://okd.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aiy.zhijiandao.cn

[I05] 按正则拆分
来源：http://auo.0kj1m.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gao.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://skd.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://qvr.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://omz.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://ose.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zna.jqgufenzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://lca.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wek.hfpthk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sut.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mzz.316326.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://crj.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ztf.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tne.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jro.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mwl.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jgf.jinghuilouyu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://arq.sxryk.cn

[I07] 忽略大小写与多行模式
来源：http://koi.52xcode.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jzs.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vyq.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tab.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://fkm.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fif.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xzl.cdnleiting.top

Ruby: s.scan(/error/i)
来源：http://pcz.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cwi.shanyushiyangtech.top

[I08] 贪婪与非贪婪匹配
来源：http://wbq.ywan-chungtsiang.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://abl.guannengcc.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iuj.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ecx.jlsjyb.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://usp.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://qyu.cashguo.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tlj.zhiwuduotai.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wtb.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://psl.jianghu66.top

================================================================================
来源：http://seb.zhaomingkeji.xyz

J. 日期与时间
来源：http://wxc.hesvh.cn

================================================================================
来源：http://zog.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://zkf.quarkkingdee.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ujr.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lgo.birdmap.top

JS:   new Date();  Date.now()
来源：http://bum.shuidangran.top

TS:   new Date();  Date.now()
来源：http://olb.jianghu66.top

Java: LocalDateTime.now();  Instant.now()
来源：http://lvt.tian-w.cn

Go:   time.Now()
来源：http://ljg.xziqi.cn

Ruby: Time.now
来源：http://itz.shangyingyoupin.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pye.hfpthk.cn

[J02] 格式化输出
来源：http://mdg.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dhu.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://trw.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pub.xuetiantiany.cn

TS:   d.toISOString()
来源：http://ftu.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hsb.hysaishi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://amj.zdqjudy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gsf.0kj1m.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uyh.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://abh.gogol.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ofn.daxiang520.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hcg.chenzaomai.com

JS:   new Date("2024-01-02")
来源：http://bwj.zhengqikj.top

TS:   new Date("2024-01-02")
来源：http://htk.zycfv.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mwd.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kbc.dianchejie.cn

Ruby: Date.parse("2024-01-02")
来源：http://cri.pengpengdd.cyou

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wyy.hnqzz.top

[J04] 时间戳与日期互转
来源：http://wgz.kuanghao11.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vko.fzhhl.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dtq.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ame.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://jka.zhijiandao.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lew.yueranfly.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uzz.guowangkeji.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xos.hnqzz.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wxw.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://bim.yj202588.top

Py:   now + timedelta(days=7)
来源：http://sru.zdbjq.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xqv.shanyushiyangkeji.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fka.hnqzz.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ssw.nanxuanxn.top

Java: LocalDate.now().plusDays(7)
来源：http://mez.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zkw.iojbl.cn

Ruby: Time.now + 7 * 86400
来源：http://hwq.shzxlz.cn

C#:   DateTime.Now.AddDays(7)
来源：http://tbs.gotoacloud.top

[J06] 计算两时间之差
来源：http://ifh.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://pvo.tanke756.top

PHP:  $end->diff($start)->days;
来源：http://xyk.dashuyun.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://liw.fktsv.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zmq.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://bvi.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://umi.fehbvm.com

Ruby: end - start                 # 返回秒数
来源：http://all.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://nvm.andypj.xyz

[J07] 比较两个日期
来源：http://mah.hesvh.cn

Py:   d1 < d2;  d1 == d2
来源：http://fkv.chenzaomai.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cra.hnxiangtu.top

JS:   d1.getTime() < d2.getTime()
来源：http://yhx.aibaodan.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yam.xuetiantiany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://azu.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vvv.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://tvl.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://kru.kuanghao11.cn

[J08] 提取年月日与星期
来源：http://xhv.zhengqikj.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gym.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://isa.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gmb.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xuk.jyoumei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tva.daria6918.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dsx.sjlbkw.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vuo.jiagoushi.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wfe.aibaodan.cn

[J09] 时区处理
来源：http://tjr.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mua.daria6918.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://dxa.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://owr.yuxming.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kbj.andypj.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jdj.yangfankeji.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kao.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://crc.wangdashe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qmf.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://tqy.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uoz.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ncx.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gfg.aizwys.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jsn.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uja.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kme.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://dll.zycfv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zby.sysykeji.top

================================================================================
来源：http://you.tarul.cn

K. JSON 与序列化
来源：http://geq.ivvv.top

================================================================================
来源：http://xwo.ywan-chungtsiang.top

[K01] 对象转 JSON 字符串
来源：http://kbs.zhixingplan.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://noc.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eav.ppjwa.cn

JS:   JSON.stringify(obj)
来源：http://nxo.ctjpmb.com

TS:   JSON.stringify(obj)
来源：http://xky.ctjpmb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fiv.guannengcc.top

Go:   json.Marshal(obj)
来源：http://ufr.yongpay.top

Ruby: obj.to_json                                     // require "json"
来源：http://usw.yonumen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://alz.uphjek.com

[K02] JSON 字符串转对象
来源：http://dkj.wangdashe.top

Py:   json.loads(s)
来源：http://est.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rxt.nanxuanxn.top

JS:   JSON.parse(s)
来源：http://zxt.sufxvd.cn

TS:   JSON.parse(s)
来源：http://zaj.chenlongwang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bjl.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://yka.0kj1m.cn

Ruby: JSON.parse(s)
来源：http://nia.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kng.wangdashe.top

[K03] JSON 美化输出（带缩进）
来源：http://nal.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://icb.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ofk.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://tur.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://utj.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ytm.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vux.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vkm.havefunace.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://csb.0kj1m.cn

[K04] 读取 JSON 文件
来源：http://hck.haohaochexian.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dyc.hammf.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://sov.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qif.shzxlz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pvd.zdqjudy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tjr.zhijiandao.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hss.yanxiufei.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://eux.shangyingyoupin.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ysc.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://dmh.9152youxi.cn

Py:   copy.deepcopy(obj)
来源：http://mgl.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://gls.52xcode.cn

JS:   structuredClone(obj)
来源：http://ihj.jqgufenzy.top

TS:   structuredClone(obj)
来源：http://ysn.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://sod.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ktg.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tdb.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mwu.hesvh.cn

[K06] 解析 URL 查询串
来源：http://yew.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gbc.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zjg.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://njt.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tzs.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jqv.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kgh.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xsy.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kpt.chenlongwang.top

[K07] 进制转换
来源：http://bhk.c1oappe.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jqc.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wyl.haohaochexian.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://upn.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ear.vqdsnc.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pdk.zhaomingkeji.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aeq.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gmn.bbcook.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nqr.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://zhx.tanke756.top

Py:   pickle.dumps(obj)
来源：http://syq.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://evf.ybcxt.top

JS:   v8.serialize(obj)        // Node
来源：http://isi.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://ads.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://iwk.fktsv.cn

Go:   encoding/gob
来源：http://mjq.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://blu.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bex.tanke756.top

================================================================================
来源：http://ygw.zhaomingkeji.xyz

L. 网络请求
来源：http://rxz.9152youxi.cn

================================================================================
来源：http://vaz.gzhubu.top

[L01] 发送 GET 请求
来源：http://prg.cheryme.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://udn.shanyushiyangkeji.top


<!-- 参考信息 -->