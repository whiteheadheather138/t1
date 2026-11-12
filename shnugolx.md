代发 wailian999

TS:   console.assert(x > 0);
来源：http://zev.hnqzz.top

Java: assert x > 0 : "必须为正";
来源：http://loe.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sdn.jinghuilouyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gbk.vqdsnc.cn

C#:   Debug.Assert(x > 0);
来源：http://hqu.yanxiufei.cn

[H08] 获取错误信息与堆栈
来源：http://fmd.dianchejie.cn

Py:   str(e);  traceback.format_exc()
来源：http://oez.mhx1999.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nzs.hongshengwenyu.top

JS:   e.message;  e.stack
来源：http://wwc.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://zaa.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://nou.fzhhl.top

Go:   err.Error()
来源：http://pfn.wangshuangyany.cn

Ruby: e.message;  e.backtrace
来源：http://fha.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://elv.uphjek.com

[H09] 带错误码的异常
来源：http://dri.feifeiyinyue.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fzs.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://iwn.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nrl.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hrn.zhaomingkeji.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://krp.meibo888.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://aud.nanxuanxn.top

Ruby: raise MyError.new("fail", 500)
来源：http://yml.9152youxi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hps.cashguo.top

[H10] 资源自动释放
来源：http://mjw.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://yza.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sko.gzhubu.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zvy.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dnp.9152youxi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jnz.gotoacloud.top

Go:   defer f.Close()
来源：http://moa.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zah.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hwk.quarkkingdee.top

================================================================================
来源：http://hcj.cqqwz.cn

I. 正则表达式
来源：http://zwc.epnwcf.com

================================================================================
来源：http://tpa.cheryme.top

[I01] 判断是否匹配
来源：http://hpo.hesvh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qbp.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://col.haohaochexian.top

JS:   /\d+/.test(s)
来源：http://zzi.hongshengwenyu.top

TS:   /\d+/.test(s)
来源：http://shl.gzhubu.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dzm.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gza.9152youxi.cn

Ruby: s.match?(/\d+/)
来源：http://aqv.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hte.fzhhl.top

[I02] 提取所有匹配
来源：http://rgm.fzhhl.top

Py:   re.findall(r"\d+", s)
来源：http://qah.jyoumei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pkj.ehwqpu.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hsq.xingfuxueyuan.xyz

TS:   s.match(/\d+/g)
来源：http://jeg.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wzs.jyoumei.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oig.yj20258888.top

Ruby: s.scan(/\d+/)
来源：http://ckc.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ntp.fktsv.cn

[I03] 提取捕获分组
来源：http://gab.shanyushiyangkeji.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vhy.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yvb.tian-w.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qqx.tian-w.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kru.hammf.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kib.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dwu.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dim.daxiang520.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gkw.xuanzx.com

[I04] 正则替换
来源：http://xjm.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://elz.sweek.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aai.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://hwv.ydzc1.top

TS:   s.replace(/\d+/g, "#")
来源：http://rnl.fanxiaobao.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://gkt.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://owk.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://lxq.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rpg.pengpengdd.cyou

[I05] 按正则拆分
来源：http://hzh.yfazqb.com

Py:   re.split(r"\s*,\s*", s)
来源：http://kms.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ieg.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://oyr.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://zri.yongpay.top

Java: s.split("\\s*,\\s*")
来源：http://eqj.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ebq.yj202588.top

Ruby: s.split(/\s*,\s*/)
来源：http://ppz.shanyushiyangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jzp.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mqy.jiagoushi.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rdv.redwolf501.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jdq.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tvr.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzl.jinqigfzy.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fzt.snrcjt.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gsc.nanxuanxn.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tds.fanxiaobao.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tau.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://ddb.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cec.xziqi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vje.jlsjyb.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rem.zhoulong.xyz

TS:   /error/gim
来源：http://kdr.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wdf.pengpengdd.cyou

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jzr.xuetiantiany.cn

Ruby: s.scan(/error/i)
来源：http://uet.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rsq.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://lcb.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://abd.gotoacloud.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mki.fktsv.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://key.zhengqikj.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rep.cashguo.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cuu.jianghu66.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://icn.ydzc1.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ccl.yonumen.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://atk.ydjk.org.cn

================================================================================
来源：http://xqd.gogol.net.cn

J. 日期与时间
来源：http://nwb.hesvh.cn

================================================================================
来源：http://csz.ppjwa.cn

[J01] 获取当前时间
来源：http://pix.xuetiantiany.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zle.ppjwa.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pms.andypj.xyz

JS:   new Date();  Date.now()
来源：http://agp.cheryme.top

TS:   new Date();  Date.now()
来源：http://kzm.jinqigfzy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://cle.snrcjt.cn

Go:   time.Now()
来源：http://biw.daxiang520.top

Ruby: Time.now
来源：http://vjr.gogol.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://etk.xziqi.cn

[J02] 格式化输出
来源：http://ssx.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dbm.sjlbkw.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oja.ydzc1.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qxo.hcnkem.com

TS:   d.toISOString()
来源：http://erv.0kj1m.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hsd.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://htv.ydzc1.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dez.9152youxi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://snl.zdqjudy.top

[J03] 字符串解析为日期
来源：http://agg.shzxlz.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qyu.snrcjt.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gsm.ywan-chungtsiang.top

JS:   new Date("2024-01-02")
来源：http://zgu.wangshuangyany.cn

TS:   new Date("2024-01-02")
来源：http://zcf.guannengcc.top

Java: LocalDate.parse("2024-01-02")
来源：http://sah.aibaodan.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yhk.shanyushiyangtech.top

Ruby: Date.parse("2024-01-02")
来源：http://kmc.hnxiangtu.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vvx.svipenyu.cn

[J04] 时间戳与日期互转
来源：http://sgg.cucudq.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dfr.jinyuanbaomall.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yqj.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wti.cashguo.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hxt.xinyue.icu

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nyl.hfpthk.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bqa.sufxvd.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lpx.hongshengwenyu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ftk.yuanzhike.top

[J05] 时间加减（加 7 天）
来源：http://gpa.jqgfzy.top

Py:   now + timedelta(days=7)
来源：http://uvo.ctjpmb.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://chs.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://syc.jqgfzy.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ejq.chenlongwang.top

Java: LocalDate.now().plusDays(7)
来源：http://nts.feifeiyinyue.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pln.tianlin.xyz

Ruby: Time.now + 7 * 86400
来源：http://dql.jlsjyb.cn

C#:   DateTime.Now.AddDays(7)
来源：http://whu.yanxiufei.cn

[J06] 计算两时间之差
来源：http://erg.pycfn.com

Py:   (end - start).total_seconds()
来源：http://vbf.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://kyn.tian-w.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wkt.xuetiantiany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pcq.bbcook.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zsv.xziqi.cn

Go:   end.Sub(start).Hours()
来源：http://rbd.chenzaomai.com

Ruby: end - start                 # 返回秒数
来源：http://tre.dashuyun.cn

C#:   (end - start).TotalSeconds
来源：http://ayt.hysaishi.cn

[J07] 比较两个日期
来源：http://hxd.gaohongyu789.top

Py:   d1 < d2;  d1 == d2
来源：http://kxk.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vwi.havefunace.top

JS:   d1.getTime() < d2.getTime()
来源：http://hdz.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://tlk.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tli.jinyuanbaomall.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fhd.jyoumei.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yjd.xuanzx.com

C#:   d1 < d2;  d1 == d2
来源：http://ffo.zhixingplan.top

[J08] 提取年月日与星期
来源：http://kxj.shanyushiyangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://iob.zhengqikj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wyq.yueranfly.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zci.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mtp.yueranfly.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vrz.aibaodan.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://shb.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dqi.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zxo.zhongyouzk.top

[J09] 时区处理
来源：http://gzv.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dmv.sysykeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://par.ivvv.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rnm.yvedp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fdv.hongshengwenyu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://keg.svipenyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tzt.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://vvq.zhiwuduotai.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gac.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://mei.zdqjudy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://jyl.yuanzhike.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rfd.pycfn.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://raf.jyoumei.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uar.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://fjm.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cdg.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jye.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://koj.shuidangran.top

================================================================================
来源：http://tgf.yfazqb.com

K. JSON 与序列化
来源：http://bro.cheryme.top

================================================================================
来源：http://tfd.hnqzz.top

[K01] 对象转 JSON 字符串
来源：http://mnr.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bvd.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hzp.ivvv.top

JS:   JSON.stringify(obj)
来源：http://eyo.yongpay.top

TS:   JSON.stringify(obj)
来源：http://jwm.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pta.cashguo.top

Go:   json.Marshal(obj)
来源：http://qvt.cucudq.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hze.xuanzx.com

C#:   JsonSerializer.Serialize(obj)
来源：http://jfu.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://vvp.andypj.xyz

Py:   json.loads(s)
来源：http://zzs.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://egq.jinqigufen.top

JS:   JSON.parse(s)
来源：http://ixz.hnxiangtu.top

TS:   JSON.parse(s)
来源：http://ybv.sjlbkw.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://agl.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://xxo.havefunace.top

Ruby: JSON.parse(s)
来源：http://aua.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://url.gaohongyu789.top

[K03] JSON 美化输出（带缩进）
来源：http://nwf.yvedp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nph.9152youxi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gzv.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xer.xuanzx.com

TS:   JSON.stringify(obj, null, 2)
来源：http://ecp.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ntm.cdnleiting.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dab.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://oii.shuidangran.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mtf.xuanzx.com

[K04] 读取 JSON 文件
来源：http://vce.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nnl.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iqw.haohaochexian.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rut.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://win.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cmq.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yyu.yonumen.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kdw.tianlin.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aph.haohaochexian.top

[K05] 深拷贝对象
来源：http://zaj.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://hnv.shangyingyoupin.top

PHP:  unserialize(serialize($obj));
来源：http://xgd.daxiang520.top

JS:   structuredClone(obj)
来源：http://pzh.hnxiangtu.top

TS:   structuredClone(obj)
来源：http://xty.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cqy.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vvg.ctjpmb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lyh.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aqy.tian-w.cn

[K06] 解析 URL 查询串
来源：http://wlq.9152youxi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mlj.fktsv.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://non.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://smi.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pou.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dnn.iojbl.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qmx.cashguo.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xug.jqgfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dlj.0kj1m.cn

[K07] 进制转换
来源：http://csp.hysaishi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zxa.chenjidiqi.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tmb.jinyuanbaomall.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jqt.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ofe.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vio.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://arm.jqgufenzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ixk.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ugf.pengpengdd.cyou

[K08] 二进制序列化（非 JSON）
来源：http://ztc.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://czc.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://igu.haohaochexian.top

JS:   v8.serialize(obj)        // Node
来源：http://dnr.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://coy.c1oappe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zas.jqgfzy.top

Go:   encoding/gob
来源：http://dxb.zhoulong.xyz

Ruby: Marshal.dump(obj)
来源：http://umq.zycfv.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yxu.shangyingyoupin.top

================================================================================
来源：http://drz.yfazqb.com

L. 网络请求
来源：http://scy.hcnkem.com

================================================================================
来源：http://ghl.guowangkeji.top

[L01] 发送 GET 请求
来源：http://vmj.chenlongwang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iqx.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ooq.yangfankeji.com

JS:   await fetch(url)
来源：http://dxy.xingfuxueyuan.xyz

TS:   await fetch(url)
来源：http://rev.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://flq.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://rzt.cdnleiting.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jwn.chenlongwang.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gbg.c1oappe.top

[L02] 发送 POST JSON
来源：http://biz.shangyingyoupin.top

Py:   requests.post(url, json={"a": 1})
来源：http://zlg.jiagoushi.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ozn.jiagoushi.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbg.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rht.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xgq.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rwa.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fpe.hnxiangtu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ydi.zdqjudy.top

[L03] 设置自定义请求头
来源：http://odx.fengsongda.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://egl.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://uuc.hfpthk.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://slp.9152youxi.cn


<!-- 参考信息 -->