代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://yyh.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://auw.havefunace.top

[H09] 带错误码的异常
来源：http://soc.tian-w.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yam.sweek.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://fsl.daria6918.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://goe.zhoulong.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zge.ctjpmb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dmu.cashguo.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wxt.hnxiangtu.top

Ruby: raise MyError.new("fail", 500)
来源：http://cmi.ctjpmb.com

C#:   // 自定义异常类中加 Code 属性
来源：http://uun.hywenlv.cn

[H10] 资源自动释放
来源：http://rrr.hammf.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zhp.zhoulong.xyz

PHP:  // 无 with：在 finally 里 fclose()
来源：http://htg.jqgufenzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://enb.aizwys.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sbi.yongpay.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tdh.ydjk.org.cn

Go:   defer f.Close()
来源：http://zal.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pqz.sufxvd.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://phi.kuanghao11.cn

================================================================================
来源：http://tbg.meibo888.top

I. 正则表达式
来源：http://ett.wangshuangyany.cn

================================================================================
来源：http://uiq.zdbjq.cn

[I01] 判断是否匹配
来源：http://etj.aibaodan.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uhj.gzhubu.top

PHP:  preg_match('/\d+/', $s);
来源：http://wlc.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://qfe.zhixingplan.top

TS:   /\d+/.test(s)
来源：http://scj.xziqi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iem.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uqt.wangdashe.top

Ruby: s.match?(/\d+/)
来源：http://ftp.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lxy.9152youxi.cn

[I02] 提取所有匹配
来源：http://myu.zhengqikj.top

Py:   re.findall(r"\d+", s)
来源：http://egv.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qyr.hysaishi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ndo.chenjidiqi.icu

TS:   s.match(/\d+/g)
来源：http://lza.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://czc.9152youxi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vzy.sweek.top

Ruby: s.scan(/\d+/)
来源：http://dfi.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pch.zhengqikj.top

[I03] 提取捕获分组
来源：http://crg.snrcjt.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nvm.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gda.ybcxt.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hyd.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://shy.tianlin.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wqg.jinyuanbaomall.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ckq.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gyn.xinyue.icu

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://raq.zhaomingkeji.xyz

[I04] 正则替换
来源：http://erp.ywan-chungtsiang.top

Py:   re.sub(r"\d+", "#", s)
来源：http://nrq.daria6918.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wxw.yueranfly.top

JS:   s.replace(/\d+/g, "#")
来源：http://vxa.snrcjt.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ccf.zhengqikj.top

Java: s.replaceAll("\\d+", "#")
来源：http://vse.redwolf501.top

Go:   re.ReplaceAllString(s, "#")
来源：http://uzz.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://bbb.haohaochexian.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://asb.gaohongyu789.top

[I05] 按正则拆分
来源：http://gsf.hfpthk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zvr.ppjwa.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mup.xuetiantiany.cn

JS:   s.split(/\s*,\s*/)
来源：http://mrm.shanyushiyangtech.top

TS:   s.split(/\s*,\s*/)
来源：http://cop.hfpthk.cn

Java: s.split("\\s*,\\s*")
来源：http://upw.havefunace.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://buj.svipenyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sbj.fktsv.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mzu.ivvv.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://smp.wangshuangyany.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bvh.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rkl.guowangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wwv.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ngo.ywan-chungtsiang.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wdb.pengpengdd.cyou

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rzd.ydzc1.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uav.guannengcc.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nlg.feifeiyinyue.top

[I07] 忽略大小写与多行模式
来源：http://tpa.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lye.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pyz.yuxming.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mna.zhoulong.xyz

TS:   /error/gim
来源：http://cbc.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fup.aizwys.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cop.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://mjs.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oxf.daria6918.cn

[I08] 贪婪与非贪婪匹配
来源：http://hny.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bvf.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://owk.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gcp.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tsl.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ebx.cqqwz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sya.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rbl.sxryk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zua.tarul.cn

================================================================================
来源：http://blc.ydzc1.top

J. 日期与时间
来源：http://doy.feifeiyinyue.top

================================================================================
来源：http://jcl.snrcjt.cn

[J01] 获取当前时间
来源：http://zei.0kj1m.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hra.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pjq.zhixingplan.top

JS:   new Date();  Date.now()
来源：http://rkr.xziqi.cn

TS:   new Date();  Date.now()
来源：http://cvp.hysaishi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://crb.chenjidiqi.icu

Go:   time.Now()
来源：http://suq.yuxming.cn

Ruby: Time.now
来源：http://qel.fehbvm.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lez.sysykeji.top

[J02] 格式化输出
来源：http://xxm.cheryme.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kcx.andypj.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hrz.0kj1m.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vsk.iojbl.cn

TS:   d.toISOString()
来源：http://amc.nwbrower.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://msy.fehbvm.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wqm.xuetiantiany.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rvj.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iur.sysykeji.top

[J03] 字符串解析为日期
来源：http://dtm.cashguo.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://amo.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xls.smart0.xyz

JS:   new Date("2024-01-02")
来源：http://onf.jqgfzy.top

TS:   new Date("2024-01-02")
来源：http://tyu.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jbn.zhixingplan.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wau.yuxming.cn

Ruby: Date.parse("2024-01-02")
来源：http://hkh.cheryme.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ryc.zhoulong.xyz

[J04] 时间戳与日期互转
来源：http://spc.tanke756.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vww.birdmap.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gaf.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://age.shuidangran.top

TS:   Math.floor(Date.now() / 1000)
来源：http://hef.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://roc.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cmt.ybcxt.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://pnu.0kj1m.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eln.hywenlv.cn

[J05] 时间加减（加 7 天）
来源：http://uoq.hnxiangtu.top

Py:   now + timedelta(days=7)
来源：http://mdv.vqdsnc.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yxz.jyoumei.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qbq.tarul.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zaf.dashuyun.cn

Java: LocalDate.now().plusDays(7)
来源：http://ywg.sjlbkw.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://noc.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://yfg.wangdashe.top

C#:   DateTime.Now.AddDays(7)
来源：http://egb.316326.xyz

[J06] 计算两时间之差
来源：http://ytb.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://upx.hysaishi.cn

PHP:  $end->diff($start)->days;
来源：http://txn.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dkk.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wgb.iojbl.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yjy.svipenyu.cn

Go:   end.Sub(start).Hours()
来源：http://eyr.jinghuilouyu.cn

Ruby: end - start                 # 返回秒数
来源：http://phh.zhoulong.xyz

C#:   (end - start).TotalSeconds
来源：http://lkp.xuanzx.com

[J07] 比较两个日期
来源：http://ibl.jinyuanbaomall.cn

Py:   d1 < d2;  d1 == d2
来源：http://mou.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ntg.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xvg.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://pfd.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vzb.316326.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mkn.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://cig.yj202588.top

C#:   d1 < d2;  d1 == d2
来源：http://fuw.yanxiufei.cn

[J08] 提取年月日与星期
来源：http://zkw.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://thu.xingfuxueyuan.xyz

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wwn.yuanzhike.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wkz.guowangkeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qfr.shzxlz.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rsf.cheryme.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ksr.hfpthk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dri.aibaodan.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rsz.dianchejie.cn

[J09] 时区处理
来源：http://dic.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://iwf.nwbrower.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ovs.svipenyu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wne.gotoacloud.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fpn.daria6918.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ltm.c1oappe.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mqm.epnwcf.com

Ruby: Time.now.getlocal("+08:00")
来源：http://bzj.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jkl.fanxiaobao.xyz

[J10] 取今天 / 本月第一天
来源：http://whs.dashuyun.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ood.andypj.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qpz.gogol.net.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ylx.hcnkem.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hok.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vkn.yanxiufei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jvu.ppjwa.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zbq.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hhh.hesvh.cn

================================================================================
来源：http://kgz.sufxvd.cn

K. JSON 与序列化
来源：http://jnm.kuanghao11.cn

================================================================================
来源：http://zur.tianlin.xyz

[K01] 对象转 JSON 字符串
来源：http://txc.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qhy.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jmy.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://ccl.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://rar.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pia.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://frt.yj20258888.top

Ruby: obj.to_json                                     // require "json"
来源：http://pgs.fzhhl.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ghv.yonumen.top

[K02] JSON 字符串转对象
来源：http://lyi.redwolf501.top

Py:   json.loads(s)
来源：http://okd.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://len.xziqi.cn

JS:   JSON.parse(s)
来源：http://ntg.yangfankeji.com

TS:   JSON.parse(s)
来源：http://kjg.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bzw.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://wfy.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://sbh.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dpy.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://zyp.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lom.yuxming.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lmo.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://irt.shanyushiyangkeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qik.yueranfly.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zmx.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://max.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://hql.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fls.quarkkingdee.top

[K04] 读取 JSON 文件
来源：http://eak.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ajb.shanyushiyangtech.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uol.chenjidiqi.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyl.jinqigufen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xwc.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ner.gzhubu.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dob.guannengcc.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cwt.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rul.xuetiantiany.cn

[K05] 深拷贝对象
来源：http://ino.yj20258.top

Py:   copy.deepcopy(obj)
来源：http://zrp.yangfankeji.com

PHP:  unserialize(serialize($obj));
来源：http://ddy.daxiang520.top

JS:   structuredClone(obj)
来源：http://tas.yueranfly.top

TS:   structuredClone(obj)
来源：http://slj.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://bgo.hnqzz.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oty.jinghuilouyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wgc.andypj.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://rls.hammf.cn

[K06] 解析 URL 查询串
来源：http://vqj.chenjidiqi.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ehi.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dwv.yj20258.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://agg.cheryme.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://khf.jqgufenzy.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mqs.yj202588.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rth.nanxuanxn.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://avh.yj202588.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xgb.guannengcc.top

[K07] 进制转换
来源：http://wfn.ehwqpu.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gbw.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vgc.sweek.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sby.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lod.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ftd.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ugu.vehdjk.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://fmd.zhoulong.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://amn.0kj1m.cn

[K08] 二进制序列化（非 JSON）
来源：http://mpa.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://qxi.fanxiaobao.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ogt.tianlin.xyz

JS:   v8.serialize(obj)        // Node
来源：http://med.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://pkh.iojbl.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jir.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://kjf.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://bkg.yuanzhike.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nor.shanyushiyangtech.top

================================================================================
来源：http://rka.xuanzx.com

L. 网络请求
来源：http://vem.hesvh.cn

================================================================================
来源：http://qrt.hywenlv.cn

[L01] 发送 GET 请求
来源：http://kts.xuanzx.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gon.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nxf.chenjidiqi.icu

JS:   await fetch(url)
来源：http://zzg.daria6918.cn

TS:   await fetch(url)
来源：http://tfs.hesvh.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ncq.dashuyun.cn

Go:   resp, err := http.Get(url)
来源：http://nxl.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fal.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ivd.vqdsnc.cn

[L02] 发送 POST JSON
来源：http://vqz.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pkg.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vyv.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://phu.fanxiaobao.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://clk.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rhx.jqgfzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zag.hnxiangtu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fcm.nanxuanxn.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jzr.hongshengwenyu.top

[L03] 设置自定义请求头
来源：http://yxp.cashguo.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hio.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://iij.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nwb.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tyd.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://czt.tarul.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nwb.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ezg.zycfv.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://maq.nanxuanxn.top

[L04] 设置超时
来源：http://cdm.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://thc.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ngz.zdqjudy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uns.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bcm.shzxlz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sdh.ybcxt.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vwd.gogol.net.cn


<!-- 参考信息 -->