代发 wailian999

TS:   console.assert(x > 0);
来源：http://hkb.daxiang520.top

Java: assert x > 0 : "必须为正";
来源：http://flq.chenzaomai.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eex.xziqi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kne.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://lkp.andypj.xyz

[H08] 获取错误信息与堆栈
来源：http://hfu.shzxlz.cn

Py:   str(e);  traceback.format_exc()
来源：http://fqy.smart0.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uyi.jinqigufen.top

JS:   e.message;  e.stack
来源：http://lrh.feifeiyinyue.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://wgs.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://juz.smart0.xyz

Go:   err.Error()
来源：http://eqm.ydzc1.top

Ruby: e.message;  e.backtrace
来源：http://ivg.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://deg.shangyingyoupin.top

[H09] 带错误码的异常
来源：http://pod.zhengqikj.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vnd.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ajt.epnwcf.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szj.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pxc.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nql.birdmap.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wkg.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://xge.ybcxt.top

C#:   // 自定义异常类中加 Code 属性
来源：http://huo.smart0.xyz

[H10] 资源自动释放
来源：http://tdr.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://kmx.xziqi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mck.zhoulong.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fhs.zhongyouzk.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lsm.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cxp.ydjk.org.cn

Go:   defer f.Close()
来源：http://byv.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wuf.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lon.hywenlv.cn

================================================================================
来源：http://ipd.xziqi.cn

I. 正则表达式
来源：http://rxd.jiagoushi.top

================================================================================
来源：http://hzv.tian-w.cn

[I01] 判断是否匹配
来源：http://mwt.haohaochexian.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mzk.hysaishi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ccq.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://ppw.tian-w.cn

TS:   /\d+/.test(s)
来源：http://zgg.iojbl.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hhb.ywan-chungtsiang.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blf.sjlbkw.cn

Ruby: s.match?(/\d+/)
来源：http://yqk.daxiang520.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wpl.sjlbkw.cn

[I02] 提取所有匹配
来源：http://ogc.ctjpmb.com

Py:   re.findall(r"\d+", s)
来源：http://fnu.sysykeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uka.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hkj.iojbl.cn

TS:   s.match(/\d+/g)
来源：http://cgz.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dso.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tgb.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://qcs.tianlin.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vkz.birdmap.top

[I03] 提取捕获分组
来源：http://gta.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xvw.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mtg.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ejx.316326.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wbg.dianchejie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wrh.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uro.daxiang520.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vdt.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://euy.sjlbkw.cn

[I04] 正则替换
来源：http://zba.nanxuanxn.top

Py:   re.sub(r"\d+", "#", s)
来源：http://hgg.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://djf.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://uvh.cucudq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dyc.yuxming.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ffk.gzhubu.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zrt.redwolf501.top

Ruby: s.gsub(/\d+/, "#")
来源：http://hwf.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://byw.zhaomingkeji.xyz

[I05] 按正则拆分
来源：http://tld.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cwf.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jzu.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://uix.ehwqpu.com

TS:   s.split(/\s*,\s*/)
来源：http://ith.zhongyouzk.top

Java: s.split("\\s*,\\s*")
来源：http://xur.yvedp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iqe.wangdashe.top

Ruby: s.split(/\s*,\s*/)
来源：http://jxj.fengsongda.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yyo.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://arl.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hlw.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ewa.jlsjyb.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nsi.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ksh.chenlongwang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://obk.vqdsnc.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://slo.yj202588.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://iby.daxiang520.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fkz.tarul.cn

[I07] 忽略大小写与多行模式
来源：http://ukb.zhaomingkeji.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hhx.iojbl.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vdb.yj20258888.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kua.aibaodan.cn

TS:   /error/gim
来源：http://orf.zhiwuduotai.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nju.jinqigfzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://myy.fehbvm.com

Ruby: s.scan(/error/i)
来源：http://gjq.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zpa.aizwys.cn

[I08] 贪婪与非贪婪匹配
来源：http://fog.haohaochexian.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ejz.tianlin.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rtq.hfpthk.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ygk.gaohongyu789.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://olx.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://fqu.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://elr.jlsjyb.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rsy.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://izv.shzxlz.cn

================================================================================
来源：http://mtf.epnwcf.com

J. 日期与时间
来源：http://nfe.pengpengdd.cyou

================================================================================
来源：http://yup.xuetiantiany.cn

[J01] 获取当前时间
来源：http://ord.ywan-chungtsiang.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://pzl.zhaomingkeji.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tzp.9152youxi.cn

JS:   new Date();  Date.now()
来源：http://ctr.shuidangran.top

TS:   new Date();  Date.now()
来源：http://tgb.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://law.shangyingyoupin.top

Go:   time.Now()
来源：http://zra.hesvh.cn

Ruby: Time.now
来源：http://cxe.xingfuxueyuan.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xiz.epnwcf.com

[J02] 格式化输出
来源：http://bmb.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kjx.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tjp.chenjidiqi.icu

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zha.daria6918.cn

TS:   d.toISOString()
来源：http://zhf.chenzaomai.com

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ycu.zdqjudy.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qlk.yuanzhike.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mxl.hnxiangtu.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fck.gaohongyu789.top

[J03] 字符串解析为日期
来源：http://swz.vqdsnc.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bdn.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ngq.yuxming.cn

JS:   new Date("2024-01-02")
来源：http://lqy.mhx1999.top

TS:   new Date("2024-01-02")
来源：http://mak.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kpx.jyoumei.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hgv.uphjek.com

Ruby: Date.parse("2024-01-02")
来源：http://kwa.jlsjyb.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fgo.yj20258888.top

[J04] 时间戳与日期互转
来源：http://oao.sjlbkw.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xsu.sufxvd.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rps.jiagoushi.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://abc.yanxiufei.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://koe.wangshuangyany.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gon.yuanzhike.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nha.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dkt.c1oappe.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kvn.shangyingyoupin.top

[J05] 时间加减（加 7 天）
来源：http://sfn.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://bmg.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ipn.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rzg.ctjpmb.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tnq.tian-w.cn

Java: LocalDate.now().plusDays(7)
来源：http://uhy.xuanzx.com

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nix.sufxvd.cn

Ruby: Time.now + 7 * 86400
来源：http://hyh.cucudq.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ueh.jinqigufen.top

[J06] 计算两时间之差
来源：http://vfj.gotoacloud.top

Py:   (end - start).total_seconds()
来源：http://ura.aibaodan.cn

PHP:  $end->diff($start)->days;
来源：http://hln.kuanghao11.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mlo.zhongyouzk.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wxr.jinqigufen.top

Java: Duration.between(start, end).toSeconds()
来源：http://uty.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://wkd.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://nro.fanxiaobao.xyz

C#:   (end - start).TotalSeconds
来源：http://tox.meibo888.top

[J07] 比较两个日期
来源：http://arf.xuanzx.com

Py:   d1 < d2;  d1 == d2
来源：http://cbl.jinqigufen.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vtk.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://cxp.jinqigufen.top

TS:   d1.getTime() < d2.getTime()
来源：http://vkb.ivvv.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gwb.guannengcc.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sdn.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://law.snrcjt.cn

C#:   d1 < d2;  d1 == d2
来源：http://yos.snrcjt.cn

[J08] 提取年月日与星期
来源：http://bwk.vehdjk.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://agf.nwbrower.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fmr.chenzaomai.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zim.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cvh.epnwcf.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://stj.yj202588.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vwk.yangfankeji.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pll.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://cde.guannengcc.top

[J09] 时区处理
来源：http://dwv.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yev.zhaomingkeji.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wtl.fehbvm.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xau.tianlin.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ymz.chenjidiqi.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ngc.tianlin.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sjx.hongshengwenyu.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ckz.c1oappe.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mje.xuetiantiany.cn

[J10] 取今天 / 本月第一天
来源：http://czq.pycfn.com

Py:   date.today();  date.today().replace(day=1)
来源：http://snv.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ukb.fktsv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qsb.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://buf.sxryk.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xms.yvedp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mpo.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ilf.hesvh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qtg.jlsjyb.cn

================================================================================
来源：http://biw.yueranfly.top

K. JSON 与序列化
来源：http://cfq.xziqi.cn

================================================================================
来源：http://nkj.yongpay.top

[K01] 对象转 JSON 字符串
来源：http://gni.ybcxt.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://chw.gogol.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ilb.ybcxt.top

JS:   JSON.stringify(obj)
来源：http://ttg.yonumen.top

TS:   JSON.stringify(obj)
来源：http://xpl.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rgz.yuxming.cn

Go:   json.Marshal(obj)
来源：http://qqd.fktsv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://wyn.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zsv.andypj.xyz

[K02] JSON 字符串转对象
来源：http://jfz.tianlin.xyz

Py:   json.loads(s)
来源：http://bdn.yfazqb.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ngw.chenjidiqi.icu

JS:   JSON.parse(s)
来源：http://zee.dashuyun.cn

TS:   JSON.parse(s)
来源：http://nvc.yueranfly.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fce.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://qca.zhixingplan.top

Ruby: JSON.parse(s)
来源：http://rnx.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cdw.birdmap.top

[K03] JSON 美化输出（带缩进）
来源：http://rse.sjlbkw.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://qib.vqdsnc.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zlq.zhongyouzk.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qbu.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://udk.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bza.epnwcf.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vjk.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://eoe.snrcjt.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iuz.ywan-chungtsiang.top

[K04] 读取 JSON 文件
来源：http://zlz.guannengcc.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eky.andypj.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iop.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bes.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uda.zhijiandao.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://epo.ywan-chungtsiang.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pbc.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bqy.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zys.9152youxi.cn

[K05] 深拷贝对象
来源：http://uhl.daria6918.cn

Py:   copy.deepcopy(obj)
来源：http://ilu.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://ngf.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://tjx.hesvh.cn

TS:   structuredClone(obj)
来源：http://doi.svipenyu.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://xlt.52xcode.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tjf.yanxiufei.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://umy.hnxiangtu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ygq.yongpay.top

[K06] 解析 URL 查询串
来源：http://zaq.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svr.chenzaomai.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ctb.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppi.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsn.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bdi.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://gvw.ctjpmb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://iwp.sweek.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wsk.sysykeji.top

[K07] 进制转换
来源：http://tie.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ejf.zhaomingkeji.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xjh.hfpthk.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ucg.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rbq.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zwx.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://twe.jianghu66.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qyk.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vyo.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://hka.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://xdf.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://lvo.zhongyouzk.top

JS:   v8.serialize(obj)        // Node
来源：http://bgl.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://mtb.xziqi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://byo.wangshuangyany.cn

Go:   encoding/gob
来源：http://kki.jiagoushi.top

Ruby: Marshal.dump(obj)
来源：http://gcc.jlsjyb.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kwe.ywan-chungtsiang.top

================================================================================
来源：http://vbp.dianchejie.cn

L. 网络请求
来源：http://eob.yvedp.cn

================================================================================
来源：http://mft.cashguo.top

[L01] 发送 GET 请求
来源：http://egn.dashuyun.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ewq.hammf.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ibo.iojbl.cn

JS:   await fetch(url)
来源：http://bvs.ehwqpu.com

TS:   await fetch(url)
来源：http://kro.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rod.jinqigfzy.top

Go:   resp, err := http.Get(url)
来源：http://yrg.guannengcc.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jif.hcnkem.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zue.zhongyouzk.top

[L02] 发送 POST JSON
来源：http://oqf.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://fgi.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zdr.xuetiantiany.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yag.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xdr.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://olw.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://okq.jinqigfzy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://iut.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rpo.cashguo.top

[L03] 设置自定义请求头
来源：http://cyw.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yhk.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zfy.jinyuanbaomall.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://enf.quarkkingdee.top


<!-- 参考信息 -->