代发 wailian999

[H07] 断言
来源：http://pio.ywan-chungtsiang.top

Py:   assert x > 0, "必须为正"
来源：http://jcx.meibo888.top

PHP:  assert($x > 0);
来源：http://fin.wangdashe.top

JS:   console.assert(x > 0);
来源：http://dzw.sxryk.cn

TS:   console.assert(x > 0);
来源：http://sdi.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://izi.fehbvm.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xzs.nanxinkj.top

Ruby: raise "必须为正" unless x > 0
来源：http://vql.zhijiandao.cn

C#:   Debug.Assert(x > 0);
来源：http://kpc.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://lnr.havefunace.top

Py:   str(e);  traceback.format_exc()
来源：http://wkx.0kj1m.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iqm.zhijiandao.cn

JS:   e.message;  e.stack
来源：http://jqi.fanxiaobao.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://ruq.sjlbkw.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kgr.guowangkeji.top

Go:   err.Error()
来源：http://rvd.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://dnb.chenzaomai.com

C#:   e.Message;  e.StackTrace
来源：http://wut.xuetiantiany.cn

[H09] 带错误码的异常
来源：http://hur.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://twk.yongpay.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bpf.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lby.zhengqikj.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mon.ydjk.org.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dya.daxiang520.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xjb.iojbl.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jxf.havefunace.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kvh.tianlin.xyz

[H10] 资源自动释放
来源：http://nzj.hnqzz.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://pxt.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gok.cucudq.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vnp.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oea.nanxuanxn.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cdz.yongpay.top

Go:   defer f.Close()
来源：http://gvz.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gab.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://klr.zhixingplan.top

================================================================================
来源：http://pda.pycfn.com

I. 正则表达式
来源：http://vgd.tarul.cn

================================================================================
来源：http://ngb.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://xcu.chenzaomai.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ovk.wangshuangyany.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gxu.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://tex.shangyingyoupin.top

TS:   /\d+/.test(s)
来源：http://irq.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://azl.dianchejie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mev.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://kko.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cdm.yuanzhike.top

[I02] 提取所有匹配
来源：http://hrf.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://dzk.havefunace.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://htw.sjlbkw.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wjb.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://quu.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qlw.bbcook.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jmb.gotoacloud.top

Ruby: s.scan(/\d+/)
来源：http://dkl.dianchejie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zit.fktsv.cn

[I03] 提取捕获分组
来源：http://ijg.hesvh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bcn.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uhq.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zsk.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://geo.nanxinkj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hmb.yvedp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xpa.smart0.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://txd.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://otz.fengsongda.top

[I04] 正则替换
来源：http://yzt.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://skx.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oar.jinqigfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://glu.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pnu.fehbvm.com

Java: s.replaceAll("\\d+", "#")
来源：http://ahp.gotoacloud.top

Go:   re.ReplaceAllString(s, "#")
来源：http://moz.daria6918.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jud.ywan-chungtsiang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://khj.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://gqb.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://szz.xinyue.icu

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://apx.yuxming.cn

JS:   s.split(/\s*,\s*/)
来源：http://klv.vehdjk.com

TS:   s.split(/\s*,\s*/)
来源：http://exd.cheryme.top

Java: s.split("\\s*,\\s*")
来源：http://bdj.tian-w.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://goq.sjlbkw.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zei.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fjf.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jrw.epnwcf.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vrr.zdqjudy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ndz.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rvh.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xbz.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cfb.hnxiangtu.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hby.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tak.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jod.hammf.cn

[I07] 忽略大小写与多行模式
来源：http://plv.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kxh.zhiwuduotai.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xkv.shzxlz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bmb.zhongyouzk.top

TS:   /error/gim
来源：http://zns.zhijiandao.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cwq.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zxe.shuidangran.top

Ruby: s.scan(/error/i)
来源：http://xzh.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qcg.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://vdc.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kyt.havefunace.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oid.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ula.yueranfly.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://shw.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://van.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xqc.c1oappe.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jmo.meibo888.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rdj.chenzaomai.com

================================================================================
来源：http://nbm.jinyuanbaomall.cn

J. 日期与时间
来源：http://kdk.nanxuanxn.top

================================================================================
来源：http://cyn.ctjpmb.com

[J01] 获取当前时间
来源：http://xxl.jinqigfzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jvn.jyoumei.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vay.jyoumei.cn

JS:   new Date();  Date.now()
来源：http://uth.sysykeji.top

TS:   new Date();  Date.now()
来源：http://nwx.smart0.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://qgq.mhx1999.top

Go:   time.Now()
来源：http://big.chenlongwang.top

Ruby: Time.now
来源：http://tnl.hongshengwenyu.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mpv.hysaishi.cn

[J02] 格式化输出
来源：http://jmq.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kjo.hcnkem.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hha.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://flf.yongpay.top

TS:   d.toISOString()
来源：http://ccl.xinyue.icu

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hqm.nanxinkj.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wvr.yj20258888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cdr.hammf.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xmz.zhoulong.xyz

[J03] 字符串解析为日期
来源：http://ohd.hnxiangtu.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wbm.andypj.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mwa.yfazqb.com

JS:   new Date("2024-01-02")
来源：http://qxi.daria6918.cn

TS:   new Date("2024-01-02")
来源：http://xqs.daria6918.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ikk.gotoacloud.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bco.vehdjk.com

Ruby: Date.parse("2024-01-02")
来源：http://rai.yfazqb.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://itl.gogol.net.cn

[J04] 时间戳与日期互转
来源：http://qsy.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xoy.nanxinkj.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wan.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jgq.jlsjyb.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jml.daria6918.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hcy.cucudq.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hwm.fanxiaobao.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xon.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ajw.gzhubu.top

[J05] 时间加减（加 7 天）
来源：http://zuw.xziqi.cn

Py:   now + timedelta(days=7)
来源：http://bmo.shuidangran.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://lnr.fengsongda.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vbl.nanxinkj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wbj.zhoulong.xyz

Java: LocalDate.now().plusDays(7)
来源：http://wju.svipenyu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zww.tarul.cn

Ruby: Time.now + 7 * 86400
来源：http://lik.uphjek.com

C#:   DateTime.Now.AddDays(7)
来源：http://zzf.andypj.xyz

[J06] 计算两时间之差
来源：http://nkp.zycfv.cn

Py:   (end - start).total_seconds()
来源：http://lsq.9152youxi.cn

PHP:  $end->diff($start)->days;
来源：http://ryu.uphjek.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bcj.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qcu.feifeiyinyue.top

Java: Duration.between(start, end).toSeconds()
来源：http://vau.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://mkb.daxiang520.top

Ruby: end - start                 # 返回秒数
来源：http://hho.gogol.net.cn

C#:   (end - start).TotalSeconds
来源：http://kbz.uphjek.com

[J07] 比较两个日期
来源：http://sof.epnwcf.com

Py:   d1 < d2;  d1 == d2
来源：http://yzm.yfazqb.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://toy.shanyushiyangtech.top

JS:   d1.getTime() < d2.getTime()
来源：http://yxd.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://cqd.nanxuanxn.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qib.nanxinkj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mcl.hnqzz.top

Ruby: d1 < d2;  d1 == d2
来源：http://sqw.vqdsnc.cn

C#:   d1 < d2;  d1 == d2
来源：http://eqh.zhiwuduotai.top

[J08] 提取年月日与星期
来源：http://mer.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nui.meibo888.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uog.ywan-chungtsiang.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hii.gogol.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xie.sjlbkw.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bpg.bbcook.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nmy.wangdashe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://csj.guowangkeji.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qmh.cqqwz.cn

[J09] 时区处理
来源：http://yxq.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ywo.hongshengwenyu.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uhr.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ieu.guowangkeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xvt.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ptk.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ynu.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://vsw.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dkc.jlsjyb.cn

[J10] 取今天 / 本月第一天
来源：http://prd.jlsjyb.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tmu.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fuk.xingfuxueyuan.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kde.pengpengdd.cyou

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://osi.jiagoushi.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ogk.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kng.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwy.zhengqikj.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qrm.chenzaomai.com

================================================================================
来源：http://rde.9152youxi.cn

K. JSON 与序列化
来源：http://dxc.yonumen.top

================================================================================
来源：http://rjw.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://muo.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hdr.aibaodan.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://owf.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://ooq.svipenyu.cn

TS:   JSON.stringify(obj)
来源：http://dva.xinyue.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lhm.yj20258888.top

Go:   json.Marshal(obj)
来源：http://vmd.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://brm.tianlin.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://zzl.shanyushiyangkeji.top

[K02] JSON 字符串转对象
来源：http://dth.chenjidiqi.icu

Py:   json.loads(s)
来源：http://mnn.zycfv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jrq.ppjwa.cn

JS:   JSON.parse(s)
来源：http://vse.cheryme.top

TS:   JSON.parse(s)
来源：http://ess.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nqw.hnqzz.top

Go:   json.Unmarshal(data, &v)
来源：http://bzk.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://rew.hywenlv.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bfi.jqgfzy.top

[K03] JSON 美化输出（带缩进）
来源：http://amy.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ono.nanxinkj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://txu.fanxiaobao.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://uxw.yuanzhike.top

TS:   JSON.stringify(obj, null, 2)
来源：http://opb.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jsi.zhoulong.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zmo.meibo888.top

Ruby: JSON.pretty_generate(obj)
来源：http://xkt.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ggq.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://zwu.jyoumei.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hop.tianlin.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lts.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://udd.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vza.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jdz.hywenlv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nky.jinghuilouyu.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qzr.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jbq.chenjidiqi.icu

[K05] 深拷贝对象
来源：http://mww.jinqigfzy.top

Py:   copy.deepcopy(obj)
来源：http://lrk.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://yet.zhijiandao.cn

JS:   structuredClone(obj)
来源：http://kpi.shanyushiyangkeji.top

TS:   structuredClone(obj)
来源：http://vxo.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://zcd.zhongyouzk.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zlb.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sxg.shzxlz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://lgo.fzhhl.top

[K06] 解析 URL 查询串
来源：http://zin.gaohongyu789.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tjp.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://cyz.hnqzz.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nbe.smart0.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nyc.xingfuxueyuan.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lgs.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://zek.jqgufenzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yml.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hgz.jqgufenzy.top

[K07] 进制转换
来源：http://fxf.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mom.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://aip.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://peg.xziqi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://khz.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ncy.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pss.nanxinkj.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nps.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://izw.gogol.net.cn

[K08] 二进制序列化（非 JSON）
来源：http://xvk.xingfuxueyuan.xyz

Py:   pickle.dumps(obj)
来源：http://qcq.sxryk.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://jrk.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://bob.zycfv.cn

TS:   v8.serialize(obj)        // Node
来源：http://jgi.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://pba.jqgfzy.top

Go:   encoding/gob
来源：http://nqu.redwolf501.top

Ruby: Marshal.dump(obj)
来源：http://bwq.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tzq.zdbjq.cn

================================================================================
来源：http://ori.xingfuxueyuan.xyz

L. 网络请求
来源：http://sof.sufxvd.cn

================================================================================
来源：http://hci.0kj1m.cn

[L01] 发送 GET 请求
来源：http://anu.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ulm.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nyk.zhiwuduotai.top

JS:   await fetch(url)
来源：http://jlr.ppjwa.cn

TS:   await fetch(url)
来源：http://hqh.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sup.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://nix.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://man.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hli.bbcook.cn

[L02] 发送 POST JSON
来源：http://xse.ydjk.org.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yiv.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://aaj.ydzc1.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fcy.yangfankeji.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hsu.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://slb.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jrr.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kae.daria6918.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ava.chenzaomai.com


<!-- 参考信息 -->