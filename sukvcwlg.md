代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://giw.c1oappe.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ixu.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cpb.ydzc1.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uei.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xxt.yanxiufei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ihd.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ksf.yuanzhike.top

[H10] 资源自动释放
来源：http://sth.yj202588.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://mdl.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qet.nwbrower.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hzj.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://csy.xylfe.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vek.jinghuilouyu.cn

Go:   defer f.Close()
来源：http://uev.cheryme.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mwd.kuanghao11.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ahp.vqdsnc.cn

================================================================================
来源：http://tpo.9152youxi.cn

I. 正则表达式
来源：http://nea.bjfxy.top

================================================================================
来源：http://lfn.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://nfa.wangshuangyany.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oeh.daxiang520.top

PHP:  preg_match('/\d+/', $s);
来源：http://idc.nwbrower.top

JS:   /\d+/.test(s)
来源：http://icx.daria6918.cn

TS:   /\d+/.test(s)
来源：http://yzz.tianlin.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nob.zdqjudy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://weg.zhiwuduotai.top

Ruby: s.match?(/\d+/)
来源：http://xox.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mgj.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://uii.ydzc1.top

Py:   re.findall(r"\d+", s)
来源：http://woj.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hvh.yanxiufei.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bke.zdqjudy.top

TS:   s.match(/\d+/g)
来源：http://juz.sweek.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://adc.jinqigufen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xmm.shuidangran.top

Ruby: s.scan(/\d+/)
来源：http://hqh.zhengqikj.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lut.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://xpj.cheryme.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zmr.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://idm.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://noe.yuanzhike.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ugo.pengpengdd.cyou

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jlh.yangfankeji.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dgh.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jfo.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://las.shzxlz.cn

[I04] 正则替换
来源：http://por.zhixingplan.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nor.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vfq.wangshuangyany.cn

JS:   s.replace(/\d+/g, "#")
来源：http://laj.ivvv.top

TS:   s.replace(/\d+/g, "#")
来源：http://ymq.fzhhl.top

Java: s.replaceAll("\\d+", "#")
来源：http://hgb.xinyue.icu

Go:   re.ReplaceAllString(s, "#")
来源：http://yyr.0kj1m.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mid.sweek.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mzg.shzxlz.cn

[I05] 按正则拆分
来源：http://cnh.smart0.xyz

Py:   re.split(r"\s*,\s*", s)
来源：http://ahn.ydjk.org.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://onq.svipenyu.cn

JS:   s.split(/\s*,\s*/)
来源：http://pjr.jinghuilouyu.cn

TS:   s.split(/\s*,\s*/)
来源：http://lxi.vehdjk.com

Java: s.split("\\s*,\\s*")
来源：http://har.gogol.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wqk.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ryy.ehwqpu.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iws.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xoj.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ekp.daxiang520.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://voj.fzhhl.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kvv.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qvg.hesvh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wxn.haohaochexian.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fvv.uphjek.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sdc.hammf.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ozp.cheryme.top

[I07] 忽略大小写与多行模式
来源：http://pnu.uphjek.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uik.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://khk.redwolf501.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sjw.shzxlz.cn

TS:   /error/gim
来源：http://bhl.guannengcc.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://omf.fzhhl.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fzp.pengpengdd.cyou

Ruby: s.scan(/error/i)
来源：http://cru.9152youxi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ndu.tianlin.xyz

[I08] 贪婪与非贪婪匹配
来源：http://umk.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fdr.sweek.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xyc.hammf.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zwl.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dlt.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://zrr.birdmap.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ypr.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qqj.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qhf.c1oappe.top

================================================================================
来源：http://tyo.wangshuangyany.cn

J. 日期与时间
来源：http://twr.yuxming.cn

================================================================================
来源：http://gpz.yvedp.cn

[J01] 获取当前时间
来源：http://uzg.zhaomingkeji.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://hdz.zhoulong.xyz

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ktx.sxryk.cn

JS:   new Date();  Date.now()
来源：http://udt.yj20258888.top

TS:   new Date();  Date.now()
来源：http://xhs.cucudq.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://beg.wangdashe.top

Go:   time.Now()
来源：http://uxt.jinghuilouyu.cn

Ruby: Time.now
来源：http://wez.cucudq.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvj.nanxinkj.top

[J02] 格式化输出
来源：http://gzx.hcnkem.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fgz.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qtm.daxiang520.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sim.shzxlz.cn

TS:   d.toISOString()
来源：http://pnf.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sio.sweek.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://guj.tianlin.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ide.yuanzhike.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://apy.hesvh.cn

[J03] 字符串解析为日期
来源：http://awx.tian-w.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ksi.xuanzx.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rlx.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://uml.c1oappe.top

TS:   new Date("2024-01-02")
来源：http://oqx.nanxuanxn.top

Java: LocalDate.parse("2024-01-02")
来源：http://jet.jiagoushi.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xxq.tarul.cn

Ruby: Date.parse("2024-01-02")
来源：http://qce.redwolf501.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ggp.tanke756.top

[J04] 时间戳与日期互转
来源：http://kyy.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iqd.bjfxy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bid.9152youxi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jpp.nwbrower.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vbg.sjlbkw.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kyn.wangshuangyany.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nbd.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mum.zhaomingkeji.xyz

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lwi.sweek.top

[J05] 时间加减（加 7 天）
来源：http://rub.yonumen.top

Py:   now + timedelta(days=7)
来源：http://gvj.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ovv.daria6918.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bmg.zhengqikj.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jfb.xziqi.cn

Java: LocalDate.now().plusDays(7)
来源：http://vkv.ydjk.org.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sbw.jlsjyb.cn

Ruby: Time.now + 7 * 86400
来源：http://koz.fanxiaobao.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sbp.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://fka.aizwys.cn

Py:   (end - start).total_seconds()
来源：http://siv.zhongyouzk.top

PHP:  $end->diff($start)->days;
来源：http://wfe.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pyw.pycfn.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://foz.zhijiandao.cn

Java: Duration.between(start, end).toSeconds()
来源：http://umy.cashguo.top

Go:   end.Sub(start).Hours()
来源：http://xje.ivvv.top

Ruby: end - start                 # 返回秒数
来源：http://ynw.daria6918.cn

C#:   (end - start).TotalSeconds
来源：http://enw.yongpay.top

[J07] 比较两个日期
来源：http://hib.mhx1999.top

Py:   d1 < d2;  d1 == d2
来源：http://cwp.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bvc.yuanzhike.top

JS:   d1.getTime() < d2.getTime()
来源：http://osk.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://jeg.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yel.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jqv.gaohongyu789.top

Ruby: d1 < d2;  d1 == d2
来源：http://jru.cdnleiting.top

C#:   d1 < d2;  d1 == d2
来源：http://alt.ywan-chungtsiang.top

[J08] 提取年月日与星期
来源：http://ksb.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kta.hywenlv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ein.fktsv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ahi.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ywk.chenzaomai.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qzd.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iet.hesvh.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lpt.fanxiaobao.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fer.sufxvd.cn

[J09] 时区处理
来源：http://jrz.316326.xyz

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yug.yuanzhike.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bel.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ktk.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zsu.yongpay.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lbd.zdbjq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tyx.feifeiyinyue.top

Ruby: Time.now.getlocal("+08:00")
来源：http://iox.cashguo.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://txm.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://yjf.316326.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://hjv.ppjwa.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lom.sjlbkw.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://aud.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://trh.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://elv.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wqf.ydzc1.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lla.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jub.gzhubu.top

================================================================================
来源：http://kyh.jinghuilouyu.cn

K. JSON 与序列化
来源：http://rga.vehdjk.com

================================================================================
来源：http://ldj.sweek.top

[K01] 对象转 JSON 字符串
来源：http://wof.ivvv.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zzm.andypj.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://udc.hesvh.cn

JS:   JSON.stringify(obj)
来源：http://xtd.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://drg.jyoumei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sfj.gotoacloud.top

Go:   json.Marshal(obj)
来源：http://deq.tanke756.top

Ruby: obj.to_json                                     // require "json"
来源：http://rdn.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://bcj.xuanzx.com

[K02] JSON 字符串转对象
来源：http://xsn.quarkkingdee.top

Py:   json.loads(s)
来源：http://mgr.jinghuilouyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mfx.zdbjq.cn

JS:   JSON.parse(s)
来源：http://hhj.dashuyun.cn

TS:   JSON.parse(s)
来源：http://icw.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fgh.zhongyouzk.top

Go:   json.Unmarshal(data, &v)
来源：http://lqr.sweek.top

Ruby: JSON.parse(s)
来源：http://izb.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ojm.yuxming.cn

[K03] JSON 美化输出（带缩进）
来源：http://vmr.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yin.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lmu.quarkkingdee.top

JS:   JSON.stringify(obj, null, 2)
来源：http://usi.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tir.xuanzx.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qdd.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://joy.gotoacloud.top

Ruby: JSON.pretty_generate(obj)
来源：http://cmb.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dxn.shanyushiyangtech.top

[K04] 读取 JSON 文件
来源：http://fmo.sweek.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cnt.chenjidiqi.icu

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zso.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gcz.svipenyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ity.uphjek.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ecp.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rxv.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://olm.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vry.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://tkd.jiagoushi.top

Py:   copy.deepcopy(obj)
来源：http://pyp.cqqwz.cn

PHP:  unserialize(serialize($obj));
来源：http://qvz.jyoumei.cn

JS:   structuredClone(obj)
来源：http://ltu.dianchejie.cn

TS:   structuredClone(obj)
来源：http://hlm.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://buh.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yeg.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lna.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://bfs.xingfuxueyuan.xyz

[K06] 解析 URL 查询串
来源：http://bzp.shzxlz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://opu.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ajo.xuetiantiany.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zey.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jmx.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lnx.svipenyu.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://jya.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nha.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ien.nanxinkj.top

[K07] 进制转换
来源：http://icp.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qcx.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hmi.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nqp.hammf.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sgc.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kqc.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mqu.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eqe.gotoacloud.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://axd.ctjpmb.com

[K08] 二进制序列化（非 JSON）
来源：http://ntj.zhijiandao.cn

Py:   pickle.dumps(obj)
来源：http://yni.vehdjk.com

PHP:  serialize($obj);  unserialize($s);
来源：http://txf.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://txg.ywan-chungtsiang.top

TS:   v8.serialize(obj)        // Node
来源：http://mxr.andypj.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jki.zhiwuduotai.top

Go:   encoding/gob
来源：http://pzp.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://vdd.dianchejie.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fvo.uphjek.com

================================================================================
来源：http://ewi.cqqwz.cn

L. 网络请求
来源：http://ket.fktsv.cn

================================================================================
来源：http://tcm.yvedp.cn

[L01] 发送 GET 请求
来源：http://ygx.shzxlz.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mng.ivvv.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qxq.316326.xyz

JS:   await fetch(url)
来源：http://nuf.zhixingplan.top

TS:   await fetch(url)
来源：http://tso.redwolf501.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hoa.zhengqikj.top

Go:   resp, err := http.Get(url)
来源：http://kea.yuanzhike.top

Ruby: Net::HTTP.get(URI(url))
来源：http://uiz.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tfz.chenzaomai.com

[L02] 发送 POST JSON
来源：http://njq.zhengqikj.top

Py:   requests.post(url, json={"a": 1})
来源：http://ykf.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://sgg.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cvl.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hrf.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://avz.dianchejie.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dvx.hysaishi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cxw.yueranfly.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dou.aibaodan.cn

[L03] 设置自定义请求头
来源：http://kxd.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ada.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eeo.pycfn.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zro.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pxe.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qgd.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ptb.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://pyi.yongpay.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ljn.shangyingyoupin.top

[L04] 设置超时
来源：http://hvf.hcnkem.com

Py:   requests.get(url, timeout=5)
来源：http://jqt.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://pyz.cucudq.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pnu.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ejn.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kuq.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bwd.mhx1999.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wvf.xuetiantiany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mmx.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://avk.sjlbkw.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xon.jqgfzy.top


<!-- 参考信息 -->