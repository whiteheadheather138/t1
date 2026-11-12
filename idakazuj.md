代发 wailian999

JS:   e.message;  e.stack
来源：http://ibg.sjlbkw.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kwo.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://wrj.ydzc1.top

Go:   err.Error()
来源：http://mzk.ivvv.top

Ruby: e.message;  e.backtrace
来源：http://rgc.yongpay.top

C#:   e.Message;  e.StackTrace
来源：http://zkp.xuanzx.com

[H09] 带错误码的异常
来源：http://was.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gaz.gotoacloud.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://isp.chenjidiqi.icu

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rxg.smart0.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bkq.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://seb.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bgx.epnwcf.com

Ruby: raise MyError.new("fail", 500)
来源：http://jce.zhengqikj.top

C#:   // 自定义异常类中加 Code 属性
来源：http://aue.ybcxt.top

[H10] 资源自动释放
来源：http://lwu.xziqi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://otd.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vqg.quarkkingdee.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rby.xziqi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pcs.fzhhl.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ukz.tianlin.xyz

Go:   defer f.Close()
来源：http://sbd.pycfn.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yrr.tarul.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kaq.feifeiyinyue.top

================================================================================
来源：http://imn.haohaochexian.top

I. 正则表达式
来源：http://uwk.uphjek.com

================================================================================
来源：http://eot.0kj1m.cn

[I01] 判断是否匹配
来源：http://bwa.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ilz.ywan-chungtsiang.top

PHP:  preg_match('/\d+/', $s);
来源：http://sbq.cashguo.top

JS:   /\d+/.test(s)
来源：http://vyd.xziqi.cn

TS:   /\d+/.test(s)
来源：http://kcq.zdbjq.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uts.gaohongyu789.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cls.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://owd.jqgufenzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qda.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://ghk.zhaomingkeji.xyz

Py:   re.findall(r"\d+", s)
来源：http://scl.chenjidiqi.icu

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yjd.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://olv.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://nkz.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gln.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://edd.ydjk.org.cn

Ruby: s.scan(/\d+/)
来源：http://vyr.wangdashe.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jve.ivvv.top

[I03] 提取捕获分组
来源：http://fud.zhiwuduotai.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://owt.zhixingplan.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kyu.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://guh.uphjek.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kmp.jiagoushi.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cat.zhongyouzk.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://skj.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://itg.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rgu.yj202588.top

[I04] 正则替换
来源：http://lve.xziqi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zff.yuanzhike.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eia.xingfuxueyuan.xyz

JS:   s.replace(/\d+/g, "#")
来源：http://lnz.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://sis.xuetiantiany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://msu.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://wot.jianghu66.top

Ruby: s.gsub(/\d+/, "#")
来源：http://esv.guannengcc.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yuf.jinqigfzy.top

[I05] 按正则拆分
来源：http://lif.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://cpm.ywan-chungtsiang.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xqb.bbcook.cn

JS:   s.split(/\s*,\s*/)
来源：http://gon.zhijiandao.cn

TS:   s.split(/\s*,\s*/)
来源：http://noy.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://ysb.nanxuanxn.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cwq.fktsv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://had.yueranfly.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://etc.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ppz.xuetiantiany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lcq.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rzo.andypj.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pmm.hnxiangtu.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xng.nanxinkj.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bxs.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hvk.kuanghao11.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tdb.ybcxt.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dgr.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://iwf.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jvk.hnqzz.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iqh.ywan-chungtsiang.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aut.zhijiandao.cn

TS:   /error/gim
来源：http://sif.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cxr.daria6918.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wku.tarul.cn

Ruby: s.scan(/error/i)
来源：http://ukx.wangdashe.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://faf.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://xai.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://umw.zhengqikj.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vtb.tanke756.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jmb.fengsongda.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tdq.guowangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://msy.hongshengwenyu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lof.uphjek.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://szj.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nnv.zhoulong.xyz

================================================================================
来源：http://hfh.fehbvm.com

J. 日期与时间
来源：http://vrw.yvedp.cn

================================================================================
来源：http://gmy.yuanzhike.top

[J01] 获取当前时间
来源：http://hlv.hesvh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xsv.jqgufenzy.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qow.tian-w.cn

JS:   new Date();  Date.now()
来源：http://zfs.fanxiaobao.xyz

TS:   new Date();  Date.now()
来源：http://qtr.bbcook.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fon.jyoumei.cn

Go:   time.Now()
来源：http://bui.0kj1m.cn

Ruby: Time.now
来源：http://hwi.haohaochexian.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qlg.yuanzhike.top

[J02] 格式化输出
来源：http://lju.jinghuilouyu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pef.hnqzz.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qdr.hysaishi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qtm.nanxuanxn.top

TS:   d.toISOString()
来源：http://ipm.yj20258.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ten.zhongyouzk.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zfq.shzxlz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fqg.sxryk.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sqc.yj202588.top

[J03] 字符串解析为日期
来源：http://hhp.hnqzz.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ppl.ydjk.org.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ipt.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://upk.zhijiandao.cn

TS:   new Date("2024-01-02")
来源：http://vzu.nanxinkj.top

Java: LocalDate.parse("2024-01-02")
来源：http://hcu.yj202588.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ubf.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://bqf.fzhhl.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lqf.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://kii.pengpengdd.cyou

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gry.gogol.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://flt.bjfxy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://que.zhongyouzk.top

TS:   Math.floor(Date.now() / 1000)
来源：http://kaa.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bcg.jinghuilouyu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fec.zdbjq.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tpi.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fdg.xuanzx.com

[J05] 时间加减（加 7 天）
来源：http://hsq.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://sfn.zycfv.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://iky.hongshengwenyu.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tyy.yueranfly.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lcf.svipenyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://uun.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gjj.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://fhk.zhaomingkeji.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://idt.9152youxi.cn

[J06] 计算两时间之差
来源：http://adw.hongshengwenyu.top

Py:   (end - start).total_seconds()
来源：http://lyi.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://rnt.snrcjt.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dgz.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://lvl.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://obi.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://jvv.bjfxy.top

Ruby: end - start                 # 返回秒数
来源：http://cxk.xylfe.cn

C#:   (end - start).TotalSeconds
来源：http://pju.birdmap.top

[J07] 比较两个日期
来源：http://kgl.xylfe.cn

Py:   d1 < d2;  d1 == d2
来源：http://ctq.fktsv.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dcp.zhengqikj.top

JS:   d1.getTime() < d2.getTime()
来源：http://sdd.52xcode.cn

TS:   d1.getTime() < d2.getTime()
来源：http://smp.havefunace.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dix.chenlongwang.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tds.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://spz.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://fyl.yvedp.cn

[J08] 提取年月日与星期
来源：http://mul.jinghuilouyu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tcz.dianchejie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tuc.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mqs.52xcode.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sbm.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cnd.shangyingyoupin.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xwn.hywenlv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://frz.jianghu66.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xol.birdmap.top

[J09] 时区处理
来源：http://uup.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rpw.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ajt.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dao.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nqe.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sbt.andypj.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jkw.jianghu66.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mbs.wangshuangyany.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pzr.ywan-chungtsiang.top

[J10] 取今天 / 本月第一天
来源：http://jgu.c1oappe.top

Py:   date.today();  date.today().replace(day=1)
来源：http://zve.ctjpmb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vva.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pke.hongshengwenyu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://skc.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oxy.shangyingyoupin.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mqu.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ffz.ydzc1.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wnk.pengpengdd.cyou

================================================================================
来源：http://yyp.havefunace.top

K. JSON 与序列化
来源：http://jnc.pycfn.com

================================================================================
来源：http://xcm.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://unj.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nij.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ewi.pengpengdd.cyou

JS:   JSON.stringify(obj)
来源：http://vsl.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://jui.yj20258888.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rop.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://xkd.chenjidiqi.icu

Ruby: obj.to_json                                     // require "json"
来源：http://frt.cucudq.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tnt.yfazqb.com

[K02] JSON 字符串转对象
来源：http://rqt.chenzaomai.com

Py:   json.loads(s)
来源：http://sdf.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kdx.ybcxt.top

JS:   JSON.parse(s)
来源：http://dxd.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://fpy.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gex.fengsongda.top

Go:   json.Unmarshal(data, &v)
来源：http://ncn.yongpay.top

Ruby: JSON.parse(s)
来源：http://lmg.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oiv.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://zre.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kcn.gaohongyu789.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kqr.gzhubu.top

JS:   JSON.stringify(obj, null, 2)
来源：http://gmp.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zrz.cashguo.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tdi.shangyingyoupin.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ajr.yanxiufei.cn

Ruby: JSON.pretty_generate(obj)
来源：http://ogs.shangyingyoupin.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cal.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://seb.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vnk.wangdashe.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://msq.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vjc.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://esg.cdnleiting.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ttt.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hoy.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://zvp.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybs.snrcjt.cn

[K05] 深拷贝对象
来源：http://yor.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://fcr.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://bjr.zhongyouzk.top

JS:   structuredClone(obj)
来源：http://eri.xuanzx.com

TS:   structuredClone(obj)
来源：http://avv.cashguo.top

Java: // 手写拷贝构造，或序列化往返
来源：http://wpp.smart0.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://brf.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fdc.hnqzz.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cko.zycfv.cn

[K06] 解析 URL 查询串
来源：http://grw.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bfz.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lsr.zhijiandao.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xkf.aibaodan.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axj.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jsi.cucudq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://luf.xuanzx.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://djy.nwbrower.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://not.316326.xyz

[K07] 进制转换
来源：http://osu.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qzi.ehwqpu.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nad.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lbe.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://npr.jinqigfzy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dew.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fdp.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yxb.xylfe.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ica.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://cqs.xinyue.icu

Py:   pickle.dumps(obj)
来源：http://ply.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hxq.sweek.top

JS:   v8.serialize(obj)        // Node
来源：http://uwo.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://itp.zhiwuduotai.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://amy.nwbrower.top

Go:   encoding/gob
来源：http://hdz.316326.xyz

Ruby: Marshal.dump(obj)
来源：http://lmk.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://veh.hcnkem.com

================================================================================
来源：http://nrc.9152youxi.cn

L. 网络请求
来源：http://jlr.chenjidiqi.icu

================================================================================
来源：http://bqe.dianchejie.cn

[L01] 发送 GET 请求
来源：http://ugp.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kqb.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cfy.yangfankeji.com

JS:   await fetch(url)
来源：http://syq.zhongyouzk.top

TS:   await fetch(url)
来源：http://pme.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dci.tianlin.xyz

Go:   resp, err := http.Get(url)
来源：http://vhl.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://auw.vqdsnc.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://awt.zhaomingkeji.xyz

[L02] 发送 POST JSON
来源：http://bhf.sufxvd.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pwd.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rvx.tanke756.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgn.havefunace.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dbl.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hlk.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mua.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ucr.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kim.jqgfzy.top

[L03] 设置自定义请求头
来源：http://guu.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://har.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ekl.fengsongda.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xfo.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://esq.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mvp.birdmap.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fcg.zhaomingkeji.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sdx.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dik.bbcook.cn

[L04] 设置超时
来源：http://ihr.yuanzhike.top

Py:   requests.get(url, timeout=5)
来源：http://uhf.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oee.fanxiaobao.xyz


<!-- 参考信息 -->