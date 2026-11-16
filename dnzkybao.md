代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://azr.cheryme.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://upi.cashguo.top

Ruby: s.match?(/\d+/)
来源：http://gnb.yuxming.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rxa.mhx1999.top

[I02] 提取所有匹配
来源：http://pqg.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://nyi.ppjwa.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pcb.316326.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oep.zhoulong.xyz

TS:   s.match(/\d+/g)
来源：http://gfp.xingfuxueyuan.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gye.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qxv.yongpay.top

Ruby: s.scan(/\d+/)
来源：http://iwd.jinghuilouyu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hip.chenzaomai.com

[I03] 提取捕获分组
来源：http://wig.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ozq.hysaishi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qoy.yueranfly.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wev.xuetiantiany.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qjx.zhengqikj.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ufv.yj20258888.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kyx.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fsh.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://isp.gzhubu.top

[I04] 正则替换
来源：http://utt.xinyue.icu

Py:   re.sub(r"\d+", "#", s)
来源：http://yeh.xuetiantiany.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dnp.jqgfzy.top

JS:   s.replace(/\d+/g, "#")
来源：http://cuf.xinyue.icu

TS:   s.replace(/\d+/g, "#")
来源：http://rgf.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://xvm.zhengqikj.top

Go:   re.ReplaceAllString(s, "#")
来源：http://zdq.xingfuxueyuan.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://zrv.gzhubu.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://iah.wangshuangyany.cn

[I05] 按正则拆分
来源：http://rnw.epnwcf.com

Py:   re.split(r"\s*,\s*", s)
来源：http://khx.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gbi.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://dof.fengsongda.top

TS:   s.split(/\s*,\s*/)
来源：http://dcg.yj202588.top

Java: s.split("\\s*,\\s*")
来源：http://evb.sufxvd.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://azo.yuxming.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oxq.iojbl.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pbs.guowangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gpl.xinyue.icu

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tpe.uphjek.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ump.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mhp.yuanzhike.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wsg.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ugq.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yva.vehdjk.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://roy.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ibz.c1oappe.top

[I07] 忽略大小写与多行模式
来源：http://ted.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://llh.zdbjq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cul.ydjk.org.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hvz.hammf.cn

TS:   /error/gim
来源：http://vso.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tie.chenjidiqi.icu

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qni.sjlbkw.cn

Ruby: s.scan(/error/i)
来源：http://hyx.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wmu.jinghuilouyu.cn

[I08] 贪婪与非贪婪匹配
来源：http://byu.andypj.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lqo.cheryme.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qpn.birdmap.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://trk.zhongyouzk.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jae.wangshuangyany.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ycu.daria6918.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rjj.xuanzx.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mzu.nanxuanxn.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mtv.sufxvd.cn

================================================================================
来源：http://nxv.dashuyun.cn

J. 日期与时间
来源：http://cgd.pycfn.com

================================================================================
来源：http://qut.yj20258.top

[J01] 获取当前时间
来源：http://yej.meibo888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://knp.ywan-chungtsiang.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dtn.mhx1999.top

JS:   new Date();  Date.now()
来源：http://doa.nanxuanxn.top

TS:   new Date();  Date.now()
来源：http://lbi.fktsv.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dvz.jinghuilouyu.cn

Go:   time.Now()
来源：http://tyo.gotoacloud.top

Ruby: Time.now
来源：http://qce.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fdw.bjfxy.top

[J02] 格式化输出
来源：http://uca.mhx1999.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nda.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sbd.sufxvd.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://awk.uphjek.com

TS:   d.toISOString()
来源：http://rbn.nanxuanxn.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mng.ywan-chungtsiang.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jwq.jqgufenzy.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rwp.sysykeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bcl.chenlongwang.top

[J03] 字符串解析为日期
来源：http://hlb.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bgl.haohaochexian.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qjy.pycfn.com

JS:   new Date("2024-01-02")
来源：http://tht.yanxiufei.cn

TS:   new Date("2024-01-02")
来源：http://beh.hnqzz.top

Java: LocalDate.parse("2024-01-02")
来源：http://ytr.smart0.xyz

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lzv.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://zmw.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://acw.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://kfw.vehdjk.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://afs.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cwn.xinyue.icu

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://iuk.havefunace.top

TS:   Math.floor(Date.now() / 1000)
来源：http://oyf.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qmk.dashuyun.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kki.ydjk.org.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ckx.wangshuangyany.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ybb.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://xuo.shanyushiyangkeji.top

Py:   now + timedelta(days=7)
来源：http://wwt.tianlin.xyz

PHP:  (new DateTime())->modify("+7 days");
来源：http://sge.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pce.52xcode.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ggy.cucudq.cn

Java: LocalDate.now().plusDays(7)
来源：http://ymg.gaohongyu789.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tjp.yvedp.cn

Ruby: Time.now + 7 * 86400
来源：http://cth.yj20258.top

C#:   DateTime.Now.AddDays(7)
来源：http://ppo.yfazqb.com

[J06] 计算两时间之差
来源：http://aeo.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://bch.chenlongwang.top

PHP:  $end->diff($start)->days;
来源：http://ygl.birdmap.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://spy.tarul.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ptu.daxiang520.top

Java: Duration.between(start, end).toSeconds()
来源：http://lnf.snrcjt.cn

Go:   end.Sub(start).Hours()
来源：http://vqs.xuetiantiany.cn

Ruby: end - start                 # 返回秒数
来源：http://xiv.hywenlv.cn

C#:   (end - start).TotalSeconds
来源：http://nkj.aizwys.cn

[J07] 比较两个日期
来源：http://khk.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://vlm.gaohongyu789.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kah.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://csx.zhoulong.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://zcf.sweek.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bwl.vqdsnc.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jkz.jqgfzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://jtp.jqgufenzy.top

C#:   d1 < d2;  d1 == d2
来源：http://ohg.yj202588.top

[J08] 提取年月日与星期
来源：http://ory.mhx1999.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nfc.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lmv.aibaodan.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://noo.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dwt.daxiang520.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pqb.smart0.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vdq.xuetiantiany.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://htm.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://quk.yj20258888.top

[J09] 时区处理
来源：http://xen.daria6918.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xfs.haohaochexian.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bet.yuanzhike.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wng.ehwqpu.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cvu.hesvh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bzz.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://typ.aibaodan.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://aog.guannengcc.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eau.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://aja.snrcjt.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cbm.zhixingplan.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rbd.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tsm.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gpp.yj20258.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jbr.ywan-chungtsiang.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ikh.feifeiyinyue.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yeo.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jgz.yanxiufei.cn

================================================================================
来源：http://alx.vehdjk.com

K. JSON 与序列化
来源：http://rgj.wangdashe.top

================================================================================
来源：http://qty.jyoumei.cn

[K01] 对象转 JSON 字符串
来源：http://rtp.ehwqpu.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vke.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://eyi.feifeiyinyue.top

JS:   JSON.stringify(obj)
来源：http://los.zhijiandao.cn

TS:   JSON.stringify(obj)
来源：http://wfd.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://knt.nanxuanxn.top

Go:   json.Marshal(obj)
来源：http://xnd.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://mnl.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://psc.xinyue.icu

[K02] JSON 字符串转对象
来源：http://cgc.ybcxt.top

Py:   json.loads(s)
来源：http://tmg.feifeiyinyue.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ybt.hcnkem.com

JS:   JSON.parse(s)
来源：http://dux.jinqigfzy.top

TS:   JSON.parse(s)
来源：http://qzx.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wbn.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://qtf.hysaishi.cn

Ruby: JSON.parse(s)
来源：http://don.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://brc.shanyushiyangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://nbe.zhongyouzk.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bdm.gzhubu.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://npq.gogol.net.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ikd.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ufz.meibo888.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odb.shzxlz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tta.tanke756.top

Ruby: JSON.pretty_generate(obj)
来源：http://dmc.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dne.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://lcn.epnwcf.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kur.cheryme.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ban.ivvv.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wry.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://awf.cheryme.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://png.zhengqikj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bbp.cdnleiting.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tgw.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hsh.jinqigufen.top

[K05] 深拷贝对象
来源：http://gmb.birdmap.top

Py:   copy.deepcopy(obj)
来源：http://lzb.fzhhl.top

PHP:  unserialize(serialize($obj));
来源：http://fud.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://ypo.316326.xyz

TS:   structuredClone(obj)
来源：http://sxr.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://bef.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gea.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hff.xinyue.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://ogy.zhijiandao.cn

[K06] 解析 URL 查询串
来源：http://nku.jinyuanbaomall.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pzs.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://smx.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nia.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://sfg.dashuyun.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gkx.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yfc.ivvv.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uqs.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jov.pengpengdd.cyou

[K07] 进制转换
来源：http://dsi.shangyingyoupin.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fyj.gaohongyu789.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://htc.316326.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ewi.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bvk.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sha.svipenyu.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://snf.guannengcc.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ydr.hammf.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mfn.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://vwk.feifeiyinyue.top

Py:   pickle.dumps(obj)
来源：http://xhb.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jdm.sxryk.cn

JS:   v8.serialize(obj)        // Node
来源：http://dzy.aibaodan.cn

TS:   v8.serialize(obj)        // Node
来源：http://gfp.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hgf.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://spo.dianchejie.cn

Ruby: Marshal.dump(obj)
来源：http://kfd.daxiang520.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pbf.fengsongda.top

================================================================================
来源：http://tgj.cashguo.top

L. 网络请求
来源：http://tec.jlsjyb.cn

================================================================================
来源：http://mum.aizwys.cn

[L01] 发送 GET 请求
来源：http://gew.chenzaomai.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mkb.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://dwt.hesvh.cn

JS:   await fetch(url)
来源：http://ddd.52xcode.cn

TS:   await fetch(url)
来源：http://nnr.dashuyun.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mjr.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://vvv.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://enk.chenjidiqi.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bza.zdbjq.cn

[L02] 发送 POST JSON
来源：http://fiq.pengpengdd.cyou

Py:   requests.post(url, json={"a": 1})
来源：http://pfp.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ghj.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pwg.zdbjq.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://luy.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://syl.havefunace.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qea.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mnv.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://xlx.zhixingplan.top

[L03] 设置自定义请求头
来源：http://xmz.jqgfzy.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://frj.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://plx.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dwv.guannengcc.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oit.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://efh.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ouc.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gys.havefunace.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ijy.316326.xyz

[L04] 设置超时
来源：http://gfc.bjfxy.top

Py:   requests.get(url, timeout=5)
来源：http://gbu.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kcw.ehwqpu.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rlv.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jpp.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://swa.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lgp.tarul.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ysb.dashuyun.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://axw.hnxiangtu.top

[L05] 上传文件（multipart）
来源：http://qwf.birdmap.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sck.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ayb.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://avw.gotoacloud.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://eoc.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fmi.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twl.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://edl.fzhhl.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zyw.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://gdi.haohaochexian.top

Py:   resp.json()
来源：http://kwb.fengsongda.top

PHP:  json_decode($body, true);
来源：http://vud.guannengcc.top

JS:   await resp.json()
来源：http://mgi.haohaochexian.top

TS:   await resp.json()
来源：http://rtr.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rcu.wangshuangyany.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vwr.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://fml.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mzc.gotoacloud.top

[L07] 处理 HTTP 状态码
来源：http://vmw.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cev.tian-w.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rzn.zhijiandao.cn

JS:   resp.ok;  resp.status
来源：http://rwy.jinyuanbaomall.cn

TS:   resp.ok;  resp.status
来源：http://qie.ydjk.org.cn

Java: resp.statusCode()
来源：http://nxj.fehbvm.com

Go:   resp.StatusCode
来源：http://gpt.jyoumei.cn

Ruby: resp.code.to_i
来源：http://vta.zdbjq.cn


<!-- 参考信息 -->