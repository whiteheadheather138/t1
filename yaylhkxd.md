代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mgc.hnxiangtu.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vlg.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://not.gotoacloud.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mcj.dashuyun.cn

[I02] 提取所有匹配
来源：http://crp.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://xjd.zhaomingkeji.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fua.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ayz.guannengcc.top

TS:   s.match(/\d+/g)
来源：http://svu.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oag.hnqzz.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qsd.ywan-chungtsiang.top

Ruby: s.scan(/\d+/)
来源：http://txg.hfpthk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ydl.redwolf501.top

[I03] 提取捕获分组
来源：http://pgs.ppjwa.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qjm.jinqigfzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ouv.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mub.tarul.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://edn.xylfe.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zni.fktsv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kxy.aibaodan.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mjn.wangdashe.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mmf.dianchejie.cn

[I04] 正则替换
来源：http://kzn.guowangkeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uoy.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hek.hongshengwenyu.top

JS:   s.replace(/\d+/g, "#")
来源：http://wvo.52xcode.cn

TS:   s.replace(/\d+/g, "#")
来源：http://emr.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iwu.sysykeji.top

Go:   re.ReplaceAllString(s, "#")
来源：http://otk.aibaodan.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xda.wangdashe.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ozi.xinyue.icu

[I05] 按正则拆分
来源：http://qvm.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://wed.jqgufenzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qfm.jinqigufen.top

JS:   s.split(/\s*,\s*/)
来源：http://ejm.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://pdm.nanxuanxn.top

Java: s.split("\\s*,\\s*")
来源：http://oit.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://prf.guowangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://yec.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hfq.chenjidiqi.icu

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bfa.jianghu66.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://esz.tanke756.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://scm.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ebq.yfazqb.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbl.xinyue.icu

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lud.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eqw.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fpy.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://shj.0kj1m.cn

[I07] 忽略大小写与多行模式
来源：http://rno.bbcook.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xal.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dbt.fanxiaobao.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ius.ydzc1.top

TS:   /error/gim
来源：http://mdr.zhongyouzk.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://idf.hywenlv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xga.tanke756.top

Ruby: s.scan(/error/i)
来源：http://fpw.epnwcf.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jqp.yvedp.cn

[I08] 贪婪与非贪婪匹配
来源：http://kxv.epnwcf.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://iwv.chenjidiqi.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yip.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lwo.bbcook.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jaq.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://fvg.shzxlz.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nfo.aibaodan.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lnd.sjlbkw.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://twe.sjlbkw.cn

================================================================================
来源：http://wck.chenzaomai.com

J. 日期与时间
来源：http://htr.guannengcc.top

================================================================================
来源：http://nwd.yuxming.cn

[J01] 获取当前时间
来源：http://tuz.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://tdo.ydjk.org.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ryc.iojbl.cn

JS:   new Date();  Date.now()
来源：http://ptp.jinqigufen.top

TS:   new Date();  Date.now()
来源：http://gcf.zhijiandao.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ujl.52xcode.cn

Go:   time.Now()
来源：http://gji.xuetiantiany.cn

Ruby: Time.now
来源：http://poe.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vda.wangdashe.top

[J02] 格式化输出
来源：http://rgs.yvedp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ikh.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zqu.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hcn.zdbjq.cn

TS:   d.toISOString()
来源：http://suq.quarkkingdee.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pjw.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kql.kuanghao11.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kqb.havefunace.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://juj.sweek.top

[J03] 字符串解析为日期
来源：http://faj.kuanghao11.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ytj.pycfn.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ham.haohaochexian.top

JS:   new Date("2024-01-02")
来源：http://ygw.hcnkem.com

TS:   new Date("2024-01-02")
来源：http://zfr.wangshuangyany.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qhh.cheryme.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://usi.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://qrw.hfpthk.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://aaz.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://anw.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vxl.bbcook.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wvh.zhengqikj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zdp.zycfv.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gcv.bjfxy.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oxu.vqdsnc.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ilu.feifeiyinyue.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gvk.redwolf501.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lir.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://juu.cheryme.top

Py:   now + timedelta(days=7)
来源：http://rlm.hysaishi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ycs.hfpthk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zpj.nwbrower.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lof.tarul.cn

Java: LocalDate.now().plusDays(7)
来源：http://wjt.zhiwuduotai.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mor.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://ujg.hnxiangtu.top

C#:   DateTime.Now.AddDays(7)
来源：http://mwq.quarkkingdee.top

[J06] 计算两时间之差
来源：http://rcj.jinqigfzy.top

Py:   (end - start).total_seconds()
来源：http://ihw.dashuyun.cn

PHP:  $end->diff($start)->days;
来源：http://loz.shuidangran.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ptf.jqgfzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tiu.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rcl.sxryk.cn

Go:   end.Sub(start).Hours()
来源：http://qxq.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://zsm.kuanghao11.cn

C#:   (end - start).TotalSeconds
来源：http://ufj.yj20258.top

[J07] 比较两个日期
来源：http://gym.yueranfly.top

Py:   d1 < d2;  d1 == d2
来源：http://uag.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rsn.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uta.gaohongyu789.top

TS:   d1.getTime() < d2.getTime()
来源：http://ldq.daxiang520.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://dcc.jianghu66.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fai.chenjidiqi.icu

Ruby: d1 < d2;  d1 == d2
来源：http://veq.bjfxy.top

C#:   d1 < d2;  d1 == d2
来源：http://hzc.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://ybs.zhaomingkeji.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fzg.mhx1999.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tyd.vqdsnc.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://obr.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nab.nwbrower.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hmn.zhongyouzk.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://iul.fengsongda.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://enx.gotoacloud.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dnx.yj20258.top

[J09] 时区处理
来源：http://dxn.ybcxt.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kce.snrcjt.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tvy.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qcv.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uzm.zhiwuduotai.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tjs.yj202588.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vea.zdbjq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://moe.ywan-chungtsiang.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fcf.hfpthk.cn

[J10] 取今天 / 本月第一天
来源：http://lqn.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dkb.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vbh.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lpa.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ibx.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dxx.shanyushiyangtech.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aum.cqqwz.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://amq.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kex.316326.xyz

================================================================================
来源：http://xfx.sxryk.cn

K. JSON 与序列化
来源：http://jly.yueranfly.top

================================================================================
来源：http://aae.ybcxt.top

[K01] 对象转 JSON 字符串
来源：http://gqd.xingfuxueyuan.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://alf.meibo888.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://adv.aizwys.cn

JS:   JSON.stringify(obj)
来源：http://ttf.jlsjyb.cn

TS:   JSON.stringify(obj)
来源：http://pui.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fdq.vehdjk.com

Go:   json.Marshal(obj)
来源：http://set.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://bgl.redwolf501.top

C#:   JsonSerializer.Serialize(obj)
来源：http://cxq.snrcjt.cn

[K02] JSON 字符串转对象
来源：http://zbr.zhengqikj.top

Py:   json.loads(s)
来源：http://zwz.yongpay.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ilh.jinghuilouyu.cn

JS:   JSON.parse(s)
来源：http://zqp.jinqigufen.top

TS:   JSON.parse(s)
来源：http://lzh.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tvr.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://guz.yvedp.cn

Ruby: JSON.parse(s)
来源：http://yfa.andypj.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zos.316326.xyz

[K03] JSON 美化输出（带缩进）
来源：http://bcw.chenjidiqi.icu

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bpm.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iaa.zhixingplan.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sia.hongshengwenyu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hpf.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://uuh.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tcc.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://lmp.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dep.vehdjk.com

[K04] 读取 JSON 文件
来源：http://aiq.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xny.jqgfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ivg.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jmi.ivvv.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vli.yongpay.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fgv.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lti.epnwcf.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://pfc.xylfe.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gzx.yonumen.top

[K05] 深拷贝对象
来源：http://bwj.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://nwk.shanyushiyangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://fxx.daxiang520.top

JS:   structuredClone(obj)
来源：http://sci.yj202588.top

TS:   structuredClone(obj)
来源：http://yla.shangyingyoupin.top

Java: // 手写拷贝构造，或序列化往返
来源：http://trj.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gaj.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://onw.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://snp.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://fim.yj20258888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fvu.haohaochexian.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lpo.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rkr.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qdw.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rez.316326.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ric.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ktk.snrcjt.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cys.ppjwa.cn

[K07] 进制转换
来源：http://drk.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://jfs.fzhhl.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bmn.jlsjyb.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vux.hfpthk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://krg.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lor.gaohongyu789.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tav.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vis.havefunace.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ftl.jinyuanbaomall.cn

[K08] 二进制序列化（非 JSON）
来源：http://hjp.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://tcv.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://hjf.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://arb.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://pmz.wangdashe.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rml.fanxiaobao.xyz

Go:   encoding/gob
来源：http://moa.zdbjq.cn

Ruby: Marshal.dump(obj)
来源：http://jlw.jqgufenzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vvz.sweek.top

================================================================================
来源：http://ihe.yfazqb.com

L. 网络请求
来源：http://jdi.hesvh.cn

================================================================================
来源：http://fbc.jiagoushi.top

[L01] 发送 GET 请求
来源：http://ujg.quarkkingdee.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mfw.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vci.ehwqpu.com

JS:   await fetch(url)
来源：http://scz.hysaishi.cn

TS:   await fetch(url)
来源：http://hbe.xylfe.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gbz.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://sdn.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rat.zhoulong.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nqq.epnwcf.com

[L02] 发送 POST JSON
来源：http://dns.xziqi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://xwv.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cou.jlsjyb.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gkb.hfpthk.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kir.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gun.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yzh.jlsjyb.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pbq.0kj1m.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vry.ydzc1.top

[L03] 设置自定义请求头
来源：http://fqe.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://seb.vqdsnc.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zxu.mhx1999.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://flc.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kkh.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ila.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qzy.zdqjudy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://diu.tarul.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fld.daxiang520.top

[L04] 设置超时
来源：http://icf.vqdsnc.cn

Py:   requests.get(url, timeout=5)
来源：http://ojf.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kmr.sxryk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zis.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tmd.yj20258.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qwo.ivvv.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sjf.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jui.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qrm.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://wdf.jianghu66.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qbs.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ipz.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ets.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vcv.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uqn.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zta.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cri.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ziu.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://srd.pycfn.com

Py:   resp.json()
来源：http://qke.ybcxt.top

PHP:  json_decode($body, true);
来源：http://mzd.zycfv.cn

JS:   await resp.json()
来源：http://vib.tian-w.cn

TS:   await resp.json()
来源：http://uru.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://yrj.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ele.dashuyun.cn

Ruby: JSON.parse(resp.body)
来源：http://rnc.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fvj.sweek.top

[L07] 处理 HTTP 状态码
来源：http://fqu.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://njs.iojbl.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nss.gzhubu.top

JS:   resp.ok;  resp.status
来源：http://fbi.yvedp.cn

TS:   resp.ok;  resp.status
来源：http://bzq.yueranfly.top

Java: resp.statusCode()
来源：http://oer.iojbl.cn

Go:   resp.StatusCode
来源：http://vev.gogol.net.cn

Ruby: resp.code.to_i
来源：http://pms.cdnleiting.top


<!-- 参考信息 -->