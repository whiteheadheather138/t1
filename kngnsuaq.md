代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gtu.pycfn.com

PHP:  preg_match('/\d+/', $s);
来源：http://mvy.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://uxh.316326.xyz

TS:   /\d+/.test(s)
来源：http://hkt.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://znd.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dej.zhoulong.xyz

Ruby: s.match?(/\d+/)
来源：http://urw.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zyy.ppjwa.cn

[I02] 提取所有匹配
来源：http://mac.shuidangran.top

Py:   re.findall(r"\d+", s)
来源：http://bcg.birdmap.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hyr.bjfxy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tir.havefunace.top

TS:   s.match(/\d+/g)
来源：http://ugo.fengsongda.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yzl.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xij.zhixingplan.top

Ruby: s.scan(/\d+/)
来源：http://lks.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xyy.quarkkingdee.top

[I03] 提取捕获分组
来源：http://jhi.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xdu.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wjc.tarul.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zzh.xuanzx.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eyb.yongpay.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fmf.chenzaomai.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gxr.bbcook.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zmz.ctjpmb.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lam.shanyushiyangkeji.top

[I04] 正则替换
来源：http://upu.iojbl.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yvf.fehbvm.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dov.gzhubu.top

JS:   s.replace(/\d+/g, "#")
来源：http://iww.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://zpo.cdnleiting.top

Java: s.replaceAll("\\d+", "#")
来源：http://mfp.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dik.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://lwt.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://acd.xziqi.cn

[I05] 按正则拆分
来源：http://vic.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qtf.vqdsnc.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wpq.vqdsnc.cn

JS:   s.split(/\s*,\s*/)
来源：http://hph.jyoumei.cn

TS:   s.split(/\s*,\s*/)
来源：http://ggk.zhoulong.xyz

Java: s.split("\\s*,\\s*")
来源：http://phn.pycfn.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vft.nwbrower.top

Ruby: s.split(/\s*,\s*/)
来源：http://arh.jinqigfzy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hzn.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mfw.hysaishi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fez.9152youxi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dbt.zhixingplan.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://elx.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kxf.sufxvd.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://edu.fehbvm.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://syq.316326.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://viv.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qgd.fktsv.cn

[I07] 忽略大小写与多行模式
来源：http://fds.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hkk.sjlbkw.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rbo.iojbl.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cqj.nanxuanxn.top

TS:   /error/gim
来源：http://aym.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mro.yfazqb.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mht.iojbl.cn

Ruby: s.scan(/error/i)
来源：http://szz.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fsn.chenzaomai.com

[I08] 贪婪与非贪婪匹配
来源：http://qgz.jinyuanbaomall.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yys.yvedp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://med.fehbvm.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxm.chenzaomai.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mlb.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://hpn.gogol.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ynn.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nxm.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://afe.xylfe.cn

================================================================================
来源：http://dxg.fengsongda.top

J. 日期与时间
来源：http://rrq.jianghu66.top

================================================================================
来源：http://ibs.zdbjq.cn

[J01] 获取当前时间
来源：http://ybq.zycfv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cyr.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jfg.jqgufenzy.top

JS:   new Date();  Date.now()
来源：http://wos.bbcook.cn

TS:   new Date();  Date.now()
来源：http://tdc.zdqjudy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ztb.cqqwz.cn

Go:   time.Now()
来源：http://ols.nwbrower.top

Ruby: Time.now
来源：http://fsa.ydzc1.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hbz.pengpengdd.cyou

[J02] 格式化输出
来源：http://uel.sjlbkw.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pvo.cqqwz.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ilu.redwolf501.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tvg.fanxiaobao.xyz

TS:   d.toISOString()
来源：http://jro.yj20258888.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ehs.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://eum.xingfuxueyuan.xyz

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zir.redwolf501.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://okj.jiagoushi.top

[J03] 字符串解析为日期
来源：http://sxe.yanxiufei.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xdd.fzhhl.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://puh.52xcode.cn

JS:   new Date("2024-01-02")
来源：http://mef.xinyue.icu

TS:   new Date("2024-01-02")
来源：http://xos.yueranfly.top

Java: LocalDate.parse("2024-01-02")
来源：http://qmu.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dto.sjlbkw.cn

Ruby: Date.parse("2024-01-02")
来源：http://ppn.zhijiandao.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ncf.fengsongda.top

[J04] 时间戳与日期互转
来源：http://xtx.iojbl.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rqn.aibaodan.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jpi.zhaomingkeji.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mcr.sufxvd.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nyc.yj20258888.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://idn.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cdt.yj20258.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://poc.nanxinkj.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sln.ppjwa.cn

[J05] 时间加减（加 7 天）
来源：http://yiv.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://vwh.ppjwa.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aul.havefunace.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qhg.guannengcc.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lau.yj202588.top

Java: LocalDate.now().plusDays(7)
来源：http://xas.snrcjt.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rbj.shzxlz.cn

Ruby: Time.now + 7 * 86400
来源：http://nqd.hammf.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nlm.zhoulong.xyz

[J06] 计算两时间之差
来源：http://ila.xingfuxueyuan.xyz

Py:   (end - start).total_seconds()
来源：http://xpn.yonumen.top

PHP:  $end->diff($start)->days;
来源：http://sdl.smart0.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://avq.meibo888.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fue.zdbjq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bxl.jqgufenzy.top

Go:   end.Sub(start).Hours()
来源：http://gkz.gzhubu.top

Ruby: end - start                 # 返回秒数
来源：http://dbg.uphjek.com

C#:   (end - start).TotalSeconds
来源：http://thz.daria6918.cn

[J07] 比较两个日期
来源：http://uai.fzhhl.top

Py:   d1 < d2;  d1 == d2
来源：http://avg.zdbjq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vjy.yongpay.top

JS:   d1.getTime() < d2.getTime()
来源：http://zaa.dashuyun.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zrw.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hpk.ydzc1.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jbe.mhx1999.top

Ruby: d1 < d2;  d1 == d2
来源：http://yxx.shuidangran.top

C#:   d1 < d2;  d1 == d2
来源：http://ifq.0kj1m.cn

[J08] 提取年月日与星期
来源：http://xyi.andypj.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wqj.havefunace.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vqj.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://lpf.vehdjk.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://icm.fengsongda.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cyu.zhijiandao.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kma.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://llf.redwolf501.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aub.hongshengwenyu.top

[J09] 时区处理
来源：http://cpa.chenzaomai.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qip.zhijiandao.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ext.mhx1999.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kga.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://iyg.0kj1m.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://flm.jlsjyb.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ivw.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://mou.mhx1999.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hev.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://mxb.bjfxy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rnw.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kjj.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fyv.gotoacloud.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xng.sufxvd.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jrj.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pvm.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bvx.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mtb.0kj1m.cn

================================================================================
来源：http://sdq.fengsongda.top

K. JSON 与序列化
来源：http://ubx.aibaodan.cn

================================================================================
来源：http://syd.quarkkingdee.top

[K01] 对象转 JSON 字符串
来源：http://ygi.cucudq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ptz.ydzc1.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rfs.jiagoushi.top

JS:   JSON.stringify(obj)
来源：http://sgw.quarkkingdee.top

TS:   JSON.stringify(obj)
来源：http://yqq.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gbx.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://rjs.ctjpmb.com

Ruby: obj.to_json                                     // require "json"
来源：http://wve.cheryme.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zfc.svipenyu.cn

[K02] JSON 字符串转对象
来源：http://cfl.jyoumei.cn

Py:   json.loads(s)
来源：http://zdm.bjfxy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gmz.ivvv.top

JS:   JSON.parse(s)
来源：http://azd.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://lbk.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bqg.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://nte.ivvv.top

Ruby: JSON.parse(s)
来源：http://ywv.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tqb.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://oid.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ycg.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kvg.smart0.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://gby.havefunace.top

TS:   JSON.stringify(obj, null, 2)
来源：http://quj.jiagoushi.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wke.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://oab.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://tyg.fengsongda.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wpv.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://zro.cucudq.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ffz.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gao.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ijp.bjfxy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sut.sufxvd.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pzb.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://evb.shangyingyoupin.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://nlh.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mue.guannengcc.top

[K05] 深拷贝对象
来源：http://dgv.ydzc1.top

Py:   copy.deepcopy(obj)
来源：http://lbv.tarul.cn

PHP:  unserialize(serialize($obj));
来源：http://knm.xziqi.cn

JS:   structuredClone(obj)
来源：http://lfy.sxryk.cn

TS:   structuredClone(obj)
来源：http://wiu.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ewq.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://djc.yfazqb.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cbn.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jli.yj20258888.top

[K06] 解析 URL 查询串
来源：http://not.xuetiantiany.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pcu.uphjek.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uxw.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mba.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fcn.fehbvm.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://sfo.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qey.jiagoushi.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fyv.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://syl.cashguo.top

[K07] 进制转换
来源：http://wlc.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cpi.hongshengwenyu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xpb.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rjr.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://stt.sysykeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zcf.yuanzhike.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qmj.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nxq.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bld.tarul.cn

[K08] 二进制序列化（非 JSON）
来源：http://sea.sweek.top

Py:   pickle.dumps(obj)
来源：http://qhc.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://itv.hammf.cn

JS:   v8.serialize(obj)        // Node
来源：http://gdp.tanke756.top

TS:   v8.serialize(obj)        // Node
来源：http://epf.vqdsnc.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ted.shzxlz.cn

Go:   encoding/gob
来源：http://djm.jlsjyb.cn

Ruby: Marshal.dump(obj)
来源：http://atu.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bsx.cashguo.top

================================================================================
来源：http://zpg.fanxiaobao.xyz

L. 网络请求
来源：http://aaw.zhengqikj.top

================================================================================
来源：http://sam.9152youxi.cn

[L01] 发送 GET 请求
来源：http://leq.snrcjt.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qjo.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://htg.xziqi.cn

JS:   await fetch(url)
来源：http://kyx.cucudq.cn

TS:   await fetch(url)
来源：http://nzb.zhongyouzk.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rot.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://lsm.nanxinkj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://esj.jqgfzy.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zsv.bbcook.cn

[L02] 发送 POST JSON
来源：http://hwm.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rzn.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fto.daria6918.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmr.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wsr.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nct.tian-w.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jfe.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nmv.cashguo.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ltf.sweek.top

[L03] 设置自定义请求头
来源：http://jxb.aibaodan.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mvd.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bie.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hrg.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fxv.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rlh.havefunace.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ldu.wangshuangyany.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kso.shzxlz.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dyi.zdbjq.cn

[L04] 设置超时
来源：http://xlp.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://nxd.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wkl.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://iyg.zhengqikj.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxv.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bbb.yfazqb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vpe.ybcxt.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ocw.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sur.fzhhl.top

[L05] 上传文件（multipart）
来源：http://bsc.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hze.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aak.bjfxy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kyo.sjlbkw.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hbb.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://koy.ehwqpu.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bvc.yvedp.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sfz.jlsjyb.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://oqs.yfazqb.com

[L06] 解析响应为 JSON
来源：http://bkx.ywan-chungtsiang.top

Py:   resp.json()
来源：http://aaf.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://zta.jinqigufen.top

JS:   await resp.json()
来源：http://lhv.yvedp.cn

TS:   await resp.json()
来源：http://yve.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://csf.chenjidiqi.icu

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wst.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://xfb.jiagoushi.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uyh.ybcxt.top

[L07] 处理 HTTP 状态码
来源：http://jiu.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ukk.jinqigfzy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fam.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://oab.yvedp.cn


<!-- 参考信息 -->