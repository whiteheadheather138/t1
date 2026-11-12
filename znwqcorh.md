代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://pvi.havefunace.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vxa.tanke756.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jay.yonumen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://iyr.xingfuxueyuan.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://elv.yj20258.top

Ruby: raise MyError.new("fail", 500)
来源：http://yui.yvedp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gcb.sweek.top

[H10] 资源自动释放
来源：http://qgw.pengpengdd.cyou

Py:   with open("a.txt") as f: data = f.read()
来源：http://ehw.yfazqb.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://siv.chenjidiqi.icu

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gje.nanxinkj.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nzz.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mrj.nanxinkj.top

Go:   defer f.Close()
来源：http://cmk.tian-w.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kib.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tpt.yfazqb.com

================================================================================
来源：http://wmq.zdqjudy.top

I. 正则表达式
来源：http://qlg.shanyushiyangkeji.top

================================================================================
来源：http://efg.hammf.cn

[I01] 判断是否匹配
来源：http://ntt.ctjpmb.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://skw.zycfv.cn

PHP:  preg_match('/\d+/', $s);
来源：http://epk.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://wql.yj20258.top

TS:   /\d+/.test(s)
来源：http://wvv.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vqp.yj202588.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dqa.ydzc1.top

Ruby: s.match?(/\d+/)
来源：http://eti.feifeiyinyue.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://peh.xinyue.icu

[I02] 提取所有匹配
来源：http://lmf.ppjwa.cn

Py:   re.findall(r"\d+", s)
来源：http://zug.sxryk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://suy.fktsv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vjc.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://rnk.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ewm.hongshengwenyu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://urt.shanyushiyangkeji.top

Ruby: s.scan(/\d+/)
来源：http://ojh.cheryme.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ies.zycfv.cn

[I03] 提取捕获分组
来源：http://tvt.zhongyouzk.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vac.sjlbkw.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zua.zhixingplan.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gsk.meibo888.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgd.pycfn.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hzd.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kkm.hammf.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qhd.xylfe.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://akp.zhijiandao.cn

[I04] 正则替换
来源：http://toz.snrcjt.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://awl.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kuv.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://fqf.hongshengwenyu.top

TS:   s.replace(/\d+/g, "#")
来源：http://zug.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hde.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://fpb.quarkkingdee.top

Ruby: s.gsub(/\d+/, "#")
来源：http://vyn.redwolf501.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kdl.gaohongyu789.top

[I05] 按正则拆分
来源：http://yhx.xinyue.icu

Py:   re.split(r"\s*,\s*", s)
来源：http://ees.yj202588.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://joj.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://nun.daxiang520.top

TS:   s.split(/\s*,\s*/)
来源：http://ffi.cqqwz.cn

Java: s.split("\\s*,\\s*")
来源：http://tak.gzhubu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gwv.xingfuxueyuan.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://ziy.daria6918.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sej.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bdj.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dty.shangyingyoupin.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ozt.vehdjk.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rzt.tanke756.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lor.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://oxa.gotoacloud.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://foy.shanyushiyangtech.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nye.yvedp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ozx.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://nte.ppjwa.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ino.quarkkingdee.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://keq.cdnleiting.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jhz.shzxlz.cn

TS:   /error/gim
来源：http://dzn.zhengqikj.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oup.tanke756.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pnt.yuanzhike.top

Ruby: s.scan(/error/i)
来源：http://qgy.cucudq.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rvr.xziqi.cn

[I08] 贪婪与非贪婪匹配
来源：http://aof.guannengcc.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://esy.kuanghao11.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yus.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tkh.52xcode.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kct.wangdashe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uno.shuidangran.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xkh.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ogi.sufxvd.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://trd.mhx1999.top

================================================================================
来源：http://hob.9152youxi.cn

J. 日期与时间
来源：http://vnq.sxryk.cn

================================================================================
来源：http://gxj.zhengqikj.top

[J01] 获取当前时间
来源：http://ltr.ydzc1.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://qik.quarkkingdee.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cac.fktsv.cn

JS:   new Date();  Date.now()
来源：http://mra.tarul.cn

TS:   new Date();  Date.now()
来源：http://eid.hfpthk.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lcr.pycfn.com

Go:   time.Now()
来源：http://qmb.vehdjk.com

Ruby: Time.now
来源：http://hzo.epnwcf.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fvj.xinyue.icu

[J02] 格式化输出
来源：http://ors.fanxiaobao.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yse.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ysk.jinyuanbaomall.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uqq.xinyue.icu

TS:   d.toISOString()
来源：http://syh.sufxvd.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gou.hfpthk.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://twm.wangshuangyany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qjy.jiagoushi.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xjy.sxryk.cn

[J03] 字符串解析为日期
来源：http://fch.zhixingplan.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lyy.c1oappe.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ffi.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://onn.iojbl.cn

TS:   new Date("2024-01-02")
来源：http://ftu.xylfe.cn

Java: LocalDate.parse("2024-01-02")
来源：http://rku.chenzaomai.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zzs.sufxvd.cn

Ruby: Date.parse("2024-01-02")
来源：http://dhx.ydzc1.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ohx.uphjek.com

[J04] 时间戳与日期互转
来源：http://hcv.daria6918.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cko.zycfv.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ggv.jqgfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wxi.andypj.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://cbi.jinqigfzy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://heb.52xcode.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qap.jinghuilouyu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gdl.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ipk.aibaodan.cn

[J05] 时间加减（加 7 天）
来源：http://ktl.fehbvm.com

Py:   now + timedelta(days=7)
来源：http://axo.jqgfzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://oti.vqdsnc.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fav.andypj.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ftj.tianlin.xyz

Java: LocalDate.now().plusDays(7)
来源：http://szn.hnxiangtu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bmj.jianghu66.top

Ruby: Time.now + 7 * 86400
来源：http://are.jinghuilouyu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://pgv.ywan-chungtsiang.top

[J06] 计算两时间之差
来源：http://hwu.shuidangran.top

Py:   (end - start).total_seconds()
来源：http://ope.hcnkem.com

PHP:  $end->diff($start)->days;
来源：http://jid.jinqigfzy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zqp.wangshuangyany.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gcv.redwolf501.top

Java: Duration.between(start, end).toSeconds()
来源：http://gij.ydzc1.top

Go:   end.Sub(start).Hours()
来源：http://jvi.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://ptz.hongshengwenyu.top

C#:   (end - start).TotalSeconds
来源：http://dpw.kuanghao11.cn

[J07] 比较两个日期
来源：http://npq.gzhubu.top

Py:   d1 < d2;  d1 == d2
来源：http://dbe.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nzs.jinqigufen.top

JS:   d1.getTime() < d2.getTime()
来源：http://ifo.sweek.top

TS:   d1.getTime() < d2.getTime()
来源：http://wtg.jlsjyb.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://whl.zhijiandao.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bve.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://xlp.aibaodan.cn

C#:   d1 < d2;  d1 == d2
来源：http://pkn.sweek.top

[J08] 提取年月日与星期
来源：http://hcb.haohaochexian.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://roz.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://myo.xuetiantiany.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hwt.yj20258888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hpa.yj20258888.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wmb.redwolf501.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vik.guannengcc.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iim.hcnkem.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ovx.zhaomingkeji.xyz

[J09] 时区处理
来源：http://jsj.9152youxi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gvt.shuidangran.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://awf.chenzaomai.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fbh.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jff.aibaodan.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eti.jyoumei.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cyv.hammf.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lgq.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wku.52xcode.cn

[J10] 取今天 / 本月第一天
来源：http://tje.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://yqm.jyoumei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://alo.tanke756.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tyi.kuanghao11.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jqd.snrcjt.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ezo.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lzz.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ejr.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://iha.zhaomingkeji.xyz

================================================================================
来源：http://vtq.nwbrower.top

K. JSON 与序列化
来源：http://gsk.yuanzhike.top

================================================================================
来源：http://rit.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://fkp.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yfg.sweek.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xaw.wangdashe.top

JS:   JSON.stringify(obj)
来源：http://nte.shangyingyoupin.top

TS:   JSON.stringify(obj)
来源：http://tvu.xylfe.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://suu.gzhubu.top

Go:   json.Marshal(obj)
来源：http://xdg.ydzc1.top

Ruby: obj.to_json                                     // require "json"
来源：http://bij.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://slx.jyoumei.cn

[K02] JSON 字符串转对象
来源：http://mzn.yangfankeji.com

Py:   json.loads(s)
来源：http://bnx.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zna.cqqwz.cn

JS:   JSON.parse(s)
来源：http://qcw.shangyingyoupin.top

TS:   JSON.parse(s)
来源：http://vnz.kuanghao11.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fda.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://iao.hcnkem.com

Ruby: JSON.parse(s)
来源：http://qcs.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ygv.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://dfv.shanyushiyangkeji.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aua.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://obs.chenlongwang.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mmh.wangshuangyany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://kfo.dianchejie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nrz.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://duk.smart0.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://nzy.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://rsn.9152youxi.cn

[K04] 读取 JSON 文件
来源：http://bhc.shanyushiyangkeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wnn.shuidangran.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yfl.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wwo.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gwb.xuanzx.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bkb.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fiq.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cyu.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ekx.c1oappe.top

[K05] 深拷贝对象
来源：http://dnw.aizwys.cn

Py:   copy.deepcopy(obj)
来源：http://pvk.meibo888.top

PHP:  unserialize(serialize($obj));
来源：http://xgj.xingfuxueyuan.xyz

JS:   structuredClone(obj)
来源：http://yup.sxryk.cn

TS:   structuredClone(obj)
来源：http://tkm.birdmap.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jqw.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wwv.xuetiantiany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ijd.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://hhr.gzhubu.top

[K06] 解析 URL 查询串
来源：http://hjd.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wlj.yongpay.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zpx.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pyo.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tpf.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oal.yj20258888.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kax.yuxming.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ajz.zdqjudy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kcd.chenzaomai.com

[K07] 进制转换
来源：http://yiq.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpo.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cuh.redwolf501.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://snp.zhoulong.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zlt.nanxuanxn.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cvd.dianchejie.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kvq.fktsv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zhn.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gkt.316326.xyz

[K08] 二进制序列化（非 JSON）
来源：http://ers.hammf.cn

Py:   pickle.dumps(obj)
来源：http://uez.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://gsw.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://wlu.daria6918.cn

TS:   v8.serialize(obj)        // Node
来源：http://tjl.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jhh.meibo888.top

Go:   encoding/gob
来源：http://cpz.fzhhl.top

Ruby: Marshal.dump(obj)
来源：http://uqh.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gpn.fehbvm.com

================================================================================
来源：http://izx.snrcjt.cn

L. 网络请求
来源：http://kwf.shangyingyoupin.top

================================================================================
来源：http://xos.snrcjt.cn

[L01] 发送 GET 请求
来源：http://psy.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yur.shanyushiyangkeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qoc.ehwqpu.com

JS:   await fetch(url)
来源：http://vcz.ybcxt.top

TS:   await fetch(url)
来源：http://aun.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mhl.daria6918.cn

Go:   resp, err := http.Get(url)
来源：http://tdn.yanxiufei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://utu.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rrq.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://xpy.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tes.vehdjk.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://btw.shanyushiyangtech.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfh.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rfl.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kiy.yongpay.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hkb.jyoumei.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vic.redwolf501.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kfe.ppjwa.cn

[L03] 设置自定义请求头
来源：http://oiy.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zos.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lch.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vvu.tanke756.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bkl.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ymu.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lrl.gotoacloud.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dym.yuanzhike.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ugt.wangshuangyany.cn

[L04] 设置超时
来源：http://gxy.feifeiyinyue.top

Py:   requests.get(url, timeout=5)
来源：http://baq.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zxd.svipenyu.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ike.cdnleiting.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://avl.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jdg.hfpthk.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xgm.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://scx.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pkd.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://fhj.pengpengdd.cyou

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qho.yueranfly.top


<!-- 参考信息 -->