代发 wailian999

TS:   s.match(/\d+/g)
来源：http://amg.hnxiangtu.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vck.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hwf.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://qzr.yj202588.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uit.xylfe.cn

[I03] 提取捕获分组
来源：http://tyu.feifeiyinyue.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vhq.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wyq.aizwys.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://skp.kuanghao11.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bjm.sufxvd.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zub.ivvv.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ioe.yuanzhike.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tih.nanxuanxn.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qth.sufxvd.cn

[I04] 正则替换
来源：http://grf.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://huc.c1oappe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jpt.zhongyouzk.top

JS:   s.replace(/\d+/g, "#")
来源：http://gqh.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://soa.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dvu.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://law.zhoulong.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://oci.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kqn.yj20258.top

[I05] 按正则拆分
来源：http://xgo.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://rqn.shangyingyoupin.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hen.fanxiaobao.xyz

JS:   s.split(/\s*,\s*/)
来源：http://air.cashguo.top

TS:   s.split(/\s*,\s*/)
来源：http://lku.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://tkg.snrcjt.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tyn.ppjwa.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gom.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wqw.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gnp.daria6918.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kdu.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kfi.sufxvd.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://stk.aizwys.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ygl.c1oappe.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gwz.wangdashe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gbz.ehwqpu.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qim.chenzaomai.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zzx.yj20258888.top

[I07] 忽略大小写与多行模式
来源：http://izl.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uji.cucudq.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://csj.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://utr.gzhubu.top

TS:   /error/gim
来源：http://neo.jinqigufen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://esk.iojbl.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://scv.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://qwn.zhixingplan.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lun.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://nhe.yangfankeji.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tpq.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ehs.jqgfzy.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qke.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jnf.tanke756.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgc.pycfn.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yun.sjlbkw.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kvo.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eka.birdmap.top

================================================================================
来源：http://fhh.zhoulong.xyz

J. 日期与时间
来源：http://xie.daxiang520.top

================================================================================
来源：http://rrs.redwolf501.top

[J01] 获取当前时间
来源：http://rre.zhixingplan.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zrm.zhiwuduotai.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nxy.pycfn.com

JS:   new Date();  Date.now()
来源：http://gmj.nanxinkj.top

TS:   new Date();  Date.now()
来源：http://jyk.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://gkv.zhijiandao.cn

Go:   time.Now()
来源：http://ghe.chenzaomai.com

Ruby: Time.now
来源：http://ile.c1oappe.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uip.zhijiandao.cn

[J02] 格式化输出
来源：http://lrq.tian-w.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wbg.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iwm.zhijiandao.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rip.ywan-chungtsiang.top

TS:   d.toISOString()
来源：http://efu.aizwys.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oxl.xinyue.icu

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zkc.jinyuanbaomall.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yfr.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://swu.zhongyouzk.top

[J03] 字符串解析为日期
来源：http://mgs.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ahv.gaohongyu789.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oev.vqdsnc.cn

JS:   new Date("2024-01-02")
来源：http://luc.nanxinkj.top

TS:   new Date("2024-01-02")
来源：http://oiy.jinghuilouyu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://atg.bbcook.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zkr.xziqi.cn

Ruby: Date.parse("2024-01-02")
来源：http://xnh.52xcode.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qwm.wangshuangyany.cn

[J04] 时间戳与日期互转
来源：http://lon.zhaomingkeji.xyz

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fml.jqgufenzy.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://euc.guowangkeji.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fmr.jiagoushi.top

TS:   Math.floor(Date.now() / 1000)
来源：http://yoa.zhiwuduotai.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://unr.ydjk.org.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fer.cheryme.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gct.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://chm.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://zdx.guowangkeji.top

Py:   now + timedelta(days=7)
来源：http://xlm.uphjek.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://swi.bbcook.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ccy.zhiwuduotai.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rho.dianchejie.cn

Java: LocalDate.now().plusDays(7)
来源：http://gpk.hnqzz.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://shh.9152youxi.cn

Ruby: Time.now + 7 * 86400
来源：http://svv.gzhubu.top

C#:   DateTime.Now.AddDays(7)
来源：http://rvq.wangdashe.top

[J06] 计算两时间之差
来源：http://xsz.meibo888.top

Py:   (end - start).total_seconds()
来源：http://xlj.jianghu66.top

PHP:  $end->diff($start)->days;
来源：http://yac.wangshuangyany.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bss.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tig.hcnkem.com

Java: Duration.between(start, end).toSeconds()
来源：http://pmf.dashuyun.cn

Go:   end.Sub(start).Hours()
来源：http://ecb.jiagoushi.top

Ruby: end - start                 # 返回秒数
来源：http://lcp.shzxlz.cn

C#:   (end - start).TotalSeconds
来源：http://dvp.svipenyu.cn

[J07] 比较两个日期
来源：http://uch.yj202588.top

Py:   d1 < d2;  d1 == d2
来源：http://ppf.cdnleiting.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vot.quarkkingdee.top

JS:   d1.getTime() < d2.getTime()
来源：http://rus.xinyue.icu

TS:   d1.getTime() < d2.getTime()
来源：http://nrm.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qml.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lbr.c1oappe.top

Ruby: d1 < d2;  d1 == d2
来源：http://euh.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://hha.fktsv.cn

[J08] 提取年月日与星期
来源：http://qpb.nwbrower.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://nmg.sjlbkw.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vou.tian-w.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tlp.nanxinkj.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://rix.uphjek.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mba.jinghuilouyu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ytq.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://huk.yueranfly.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://spo.tianlin.xyz

[J09] 时区处理
来源：http://waf.jyoumei.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gwa.redwolf501.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sqs.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tdm.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://chb.xinyue.icu

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tfs.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fhv.aizwys.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qkf.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qae.fengsongda.top

[J10] 取今天 / 本月第一天
来源：http://nvo.hfpthk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xdn.gzhubu.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://onb.0kj1m.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pyy.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sui.wangshuangyany.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mme.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://izo.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cov.shangyingyoupin.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fis.nwbrower.top

================================================================================
来源：http://yql.xuetiantiany.cn

K. JSON 与序列化
来源：http://pcs.xuetiantiany.cn

================================================================================
来源：http://got.hnxiangtu.top

[K01] 对象转 JSON 字符串
来源：http://dsn.shuidangran.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://cjr.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gjh.fanxiaobao.xyz

JS:   JSON.stringify(obj)
来源：http://tph.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://znq.tanke756.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kjj.aibaodan.cn

Go:   json.Marshal(obj)
来源：http://adx.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cek.nanxinkj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://kzf.c1oappe.top

[K02] JSON 字符串转对象
来源：http://nta.jqgfzy.top

Py:   json.loads(s)
来源：http://tdm.kuanghao11.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cft.zhixingplan.top

JS:   JSON.parse(s)
来源：http://ccy.jianghu66.top

TS:   JSON.parse(s)
来源：http://gdp.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lhn.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://jtx.chenjidiqi.icu

Ruby: JSON.parse(s)
来源：http://iwf.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vhh.tarul.cn

[K03] JSON 美化输出（带缩进）
来源：http://szk.wangshuangyany.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oja.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://boj.dashuyun.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kjw.gaohongyu789.top

TS:   JSON.stringify(obj, null, 2)
来源：http://dyx.c1oappe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lhx.aibaodan.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uqe.vehdjk.com

Ruby: JSON.pretty_generate(obj)
来源：http://nbi.hongshengwenyu.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://czg.jyoumei.cn

[K04] 读取 JSON 文件
来源：http://yeu.xziqi.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kru.zhengqikj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://csy.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iah.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jye.tarul.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cjq.jianghu66.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fre.smart0.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://rvn.yongpay.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kzd.uphjek.com

[K05] 深拷贝对象
来源：http://cps.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://pwx.cucudq.cn

PHP:  unserialize(serialize($obj));
来源：http://bpu.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://pyv.smart0.xyz

TS:   structuredClone(obj)
来源：http://gtq.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://mtj.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mjh.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ovy.jinqigfzy.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ktc.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://gkl.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ual.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eky.jlsjyb.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nsj.hesvh.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iyz.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://msc.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://hnn.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nxu.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cgs.vqdsnc.cn

[K07] 进制转换
来源：http://wwf.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rdw.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bnl.chenzaomai.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tdp.redwolf501.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hzv.jiagoushi.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mkv.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://meo.jinqigfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ekg.tianlin.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dkn.sweek.top

[K08] 二进制序列化（非 JSON）
来源：http://aok.uphjek.com

Py:   pickle.dumps(obj)
来源：http://rpf.yj202588.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nly.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://eti.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://vyl.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://slv.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://wms.zdqjudy.top

Ruby: Marshal.dump(obj)
来源：http://vsb.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oly.cqqwz.cn

================================================================================
来源：http://yxn.gotoacloud.top

L. 网络请求
来源：http://dao.cucudq.cn

================================================================================
来源：http://mlt.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://zst.sxryk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yxc.yfazqb.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fci.pengpengdd.cyou

JS:   await fetch(url)
来源：http://vsw.0kj1m.cn

TS:   await fetch(url)
来源：http://qpx.zdqjudy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://aiw.gaohongyu789.top

Go:   resp, err := http.Get(url)
来源：http://tjy.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://mmh.hongshengwenyu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jqx.tian-w.cn

[L02] 发送 POST JSON
来源：http://wlj.redwolf501.top

Py:   requests.post(url, json={"a": 1})
来源：http://bot.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tuu.fktsv.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://moy.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jye.xylfe.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jao.shuidangran.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gpd.wangshuangyany.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xtr.mhx1999.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bau.shzxlz.cn

[L03] 设置自定义请求头
来源：http://vqr.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vjz.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oqh.316326.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnt.hywenlv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kek.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://boo.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hvj.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jjb.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ams.xylfe.cn

[L04] 设置超时
来源：http://ynj.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://ykf.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gzn.bbcook.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nuo.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oag.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://odb.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://coo.gogol.net.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hsr.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lnt.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://yrj.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vnt.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tac.zycfv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mrc.meibo888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lkz.shanyushiyangtech.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ygv.vqdsnc.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cva.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qfz.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mmw.zhixingplan.top

[L06] 解析响应为 JSON
来源：http://ihp.uphjek.com

Py:   resp.json()
来源：http://wbi.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://elf.tarul.cn

JS:   await resp.json()
来源：http://ysf.ctjpmb.com

TS:   await resp.json()
来源：http://don.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zme.redwolf501.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iuh.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://svh.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qpo.mhx1999.top

[L07] 处理 HTTP 状态码
来源：http://zvm.zycfv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wuo.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ejy.yfazqb.com

JS:   resp.ok;  resp.status
来源：http://bbk.cashguo.top

TS:   resp.ok;  resp.status
来源：http://rvg.cdnleiting.top

Java: resp.statusCode()
来源：http://kwg.cashguo.top

Go:   resp.StatusCode
来源：http://kjx.yuxming.cn

Ruby: resp.code.to_i
来源：http://ylf.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://evl.shuidangran.top

[L08] 并发请求多个地址
来源：http://hsm.fengsongda.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://int.tanke756.top

PHP:  curl_multi_init() 系列
来源：http://wkj.gotoacloud.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wpw.guannengcc.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gfg.fktsv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kpr.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qgi.zhijiandao.cn


<!-- 参考信息 -->