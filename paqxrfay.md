代发 wailian999

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hfw.316326.xyz

[I03] 提取捕获分组
来源：http://hpb.bbcook.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://csm.cdnleiting.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://icp.cheryme.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://onp.fktsv.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iff.fanxiaobao.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qvj.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kfz.xuanzx.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jxj.yanxiufei.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pja.meibo888.top

[I04] 正则替换
来源：http://huc.uphjek.com

Py:   re.sub(r"\d+", "#", s)
来源：http://vaa.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://aqt.chenzaomai.com

JS:   s.replace(/\d+/g, "#")
来源：http://slb.shanyushiyangtech.top

TS:   s.replace(/\d+/g, "#")
来源：http://ulf.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://xge.jinqigfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://qot.ywan-chungtsiang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://aox.9152youxi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xml.aibaodan.cn

[I05] 按正则拆分
来源：http://urx.jiagoushi.top

Py:   re.split(r"\s*,\s*", s)
来源：http://aek.xylfe.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cfr.guannengcc.top

JS:   s.split(/\s*,\s*/)
来源：http://kyj.hnxiangtu.top

TS:   s.split(/\s*,\s*/)
来源：http://zau.zycfv.cn

Java: s.split("\\s*,\\s*")
来源：http://gwk.tianlin.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fhi.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://rgq.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dni.jinghuilouyu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rem.dianchejie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rfg.xylfe.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kge.iojbl.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dif.zhijiandao.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mda.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cmn.hywenlv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iuj.nanxinkj.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bry.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://syf.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://bte.jinqigufen.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://amg.zhijiandao.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nvg.cqqwz.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xsy.zhengqikj.top

TS:   /error/gim
来源：http://yeb.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fbv.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ewk.52xcode.cn

Ruby: s.scan(/error/i)
来源：http://kiv.hongshengwenyu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ebj.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://pot.cheryme.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uyt.haohaochexian.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qkx.smart0.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqv.zhaomingkeji.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mtc.bjfxy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yam.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lif.jianghu66.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pgb.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ijw.kuanghao11.cn

================================================================================
来源：http://gdw.gaohongyu789.top

J. 日期与时间
来源：http://brd.dashuyun.cn

================================================================================
来源：http://wyq.gotoacloud.top

[J01] 获取当前时间
来源：http://sgu.nwbrower.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://zir.chenjidiqi.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dqp.andypj.xyz

JS:   new Date();  Date.now()
来源：http://wds.jinqigfzy.top

TS:   new Date();  Date.now()
来源：http://dqg.hongshengwenyu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ock.tanke756.top

Go:   time.Now()
来源：http://akd.yj20258.top

Ruby: Time.now
来源：http://bvi.nanxuanxn.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cvt.0kj1m.cn

[J02] 格式化输出
来源：http://kqu.vehdjk.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eji.shanyushiyangtech.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xcm.feifeiyinyue.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fms.yangfankeji.com

TS:   d.toISOString()
来源：http://rjb.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gpu.hcnkem.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lih.svipenyu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://efn.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mbt.yj202588.top

[J03] 字符串解析为日期
来源：http://bzb.aibaodan.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ygl.zhiwuduotai.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://evg.jyoumei.cn

JS:   new Date("2024-01-02")
来源：http://hzp.yj202588.top

TS:   new Date("2024-01-02")
来源：http://cgd.hesvh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kum.yonumen.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qbe.smart0.xyz

Ruby: Date.parse("2024-01-02")
来源：http://rxc.fehbvm.com

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tsb.sjlbkw.cn

[J04] 时间戳与日期互转
来源：http://wpr.fzhhl.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jwq.meibo888.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fdb.fanxiaobao.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mvz.ydjk.org.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://uds.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kif.zhijiandao.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jfo.yuxming.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://skr.xinyue.icu

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://imx.uphjek.com

[J05] 时间加减（加 7 天）
来源：http://xff.svipenyu.cn

Py:   now + timedelta(days=7)
来源：http://bug.dashuyun.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yps.ywan-chungtsiang.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ohh.sysykeji.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://psw.epnwcf.com

Java: LocalDate.now().plusDays(7)
来源：http://flw.yj20258888.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qrs.guannengcc.top

Ruby: Time.now + 7 * 86400
来源：http://wrg.dashuyun.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gjg.wangdashe.top

[J06] 计算两时间之差
来源：http://vnw.9152youxi.cn

Py:   (end - start).total_seconds()
来源：http://fez.hongshengwenyu.top

PHP:  $end->diff($start)->days;
来源：http://wmy.aizwys.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gtd.cheryme.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rgw.ybcxt.top

Java: Duration.between(start, end).toSeconds()
来源：http://nri.wangdashe.top

Go:   end.Sub(start).Hours()
来源：http://pig.nanxuanxn.top

Ruby: end - start                 # 返回秒数
来源：http://qgi.chenjidiqi.icu

C#:   (end - start).TotalSeconds
来源：http://iwz.yuanzhike.top

[J07] 比较两个日期
来源：http://std.zhaomingkeji.xyz

Py:   d1 < d2;  d1 == d2
来源：http://vor.mhx1999.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://amc.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://wqb.jqgfzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://avn.chenlongwang.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mjm.0kj1m.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bta.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mca.xziqi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ftb.dashuyun.cn

[J08] 提取年月日与星期
来源：http://jby.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yrn.zhiwuduotai.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tam.daria6918.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wjk.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sml.zhoulong.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jae.hongshengwenyu.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ooq.xinyue.icu

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yll.xingfuxueyuan.xyz

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tnt.jyoumei.cn

[J09] 时区处理
来源：http://ipy.cdnleiting.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hka.yvedp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fqp.sxryk.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vaz.yueranfly.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hgs.hnqzz.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://urn.cucudq.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hsq.chenjidiqi.icu

Ruby: Time.now.getlocal("+08:00")
来源：http://cjf.daxiang520.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qxb.yanxiufei.cn

[J10] 取今天 / 本月第一天
来源：http://lcu.daria6918.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://frt.fktsv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ttt.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kon.jlsjyb.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://czz.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zvt.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xrz.xziqi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lyf.sufxvd.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://avq.sysykeji.top

================================================================================
来源：http://tbt.yj202588.top

K. JSON 与序列化
来源：http://kla.fanxiaobao.xyz

================================================================================
来源：http://xtp.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://wxt.yuxming.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://msu.tanke756.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nyn.jinqigfzy.top

JS:   JSON.stringify(obj)
来源：http://esh.jiagoushi.top

TS:   JSON.stringify(obj)
来源：http://jab.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ueu.fehbvm.com

Go:   json.Marshal(obj)
来源：http://ivq.epnwcf.com

Ruby: obj.to_json                                     // require "json"
来源：http://izs.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj)
来源：http://imh.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://azk.fengsongda.top

Py:   json.loads(s)
来源：http://hgx.c1oappe.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xjr.hnxiangtu.top

JS:   JSON.parse(s)
来源：http://wvc.ydzc1.top

TS:   JSON.parse(s)
来源：http://rup.pycfn.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://geu.hesvh.cn

Go:   json.Unmarshal(data, &v)
来源：http://qqv.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://cis.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://elg.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://lcv.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://myf.ivvv.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zfb.sxryk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qwf.smart0.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://hbe.yfazqb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wqy.jqgfzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ulu.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://qop.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lzu.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://zkg.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cuf.0kj1m.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uhq.shangyingyoupin.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sty.jlsjyb.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rgo.daria6918.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dml.tianlin.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hta.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://xti.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cju.gzhubu.top

[K05] 深拷贝对象
来源：http://tdu.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://sdg.xuetiantiany.cn

PHP:  unserialize(serialize($obj));
来源：http://nox.sxryk.cn

JS:   structuredClone(obj)
来源：http://tqc.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://hjp.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rag.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://llu.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xiy.uphjek.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ubk.xuanzx.com

[K06] 解析 URL 查询串
来源：http://hez.hnxiangtu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ugs.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://urs.gotoacloud.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://dwk.snrcjt.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xuj.ybcxt.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fdm.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tvs.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://quu.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gxq.tianlin.xyz

[K07] 进制转换
来源：http://lxr.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://kvg.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://glo.fengsongda.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xtp.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qwc.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rlm.0kj1m.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nla.fengsongda.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qkt.vqdsnc.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zhr.xziqi.cn

[K08] 二进制序列化（非 JSON）
来源：http://aaq.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://txh.nwbrower.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ckw.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://xwq.dianchejie.cn

TS:   v8.serialize(obj)        // Node
来源：http://hac.52xcode.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xqx.quarkkingdee.top

Go:   encoding/gob
来源：http://dkt.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://nss.havefunace.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://isd.jianghu66.top

================================================================================
来源：http://bta.52xcode.cn

L. 网络请求
来源：http://jmx.cashguo.top

================================================================================
来源：http://plx.tianlin.xyz

[L01] 发送 GET 请求
来源：http://muj.jinqigfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xhl.hysaishi.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://zqp.cqqwz.cn

JS:   await fetch(url)
来源：http://ihs.svipenyu.cn

TS:   await fetch(url)
来源：http://hle.316326.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yet.snrcjt.cn

Go:   resp, err := http.Get(url)
来源：http://mlf.xinyue.icu

Ruby: Net::HTTP.get(URI(url))
来源：http://avo.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://byu.yueranfly.top

[L02] 发送 POST JSON
来源：http://ake.wangdashe.top

Py:   requests.post(url, json={"a": 1})
来源：http://qlj.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vto.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gcl.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://crj.zdqjudy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://sza.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qvg.gzhubu.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wwt.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lui.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://jaq.daxiang520.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xha.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qhc.daxiang520.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rog.wangdashe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kte.jinqigufen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tlr.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ybu.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rix.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jgz.fktsv.cn

[L04] 设置超时
来源：http://iyq.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://ecb.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lpo.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bnf.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://upx.gaohongyu789.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rlv.fzhhl.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://edn.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rcm.nanxinkj.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://poi.cheryme.top

[L05] 上传文件（multipart）
来源：http://zpa.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ecn.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gty.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dde.shangyingyoupin.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pkc.sysykeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rvn.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rhs.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ojh.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gyo.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://flc.shanyushiyangtech.top

Py:   resp.json()
来源：http://jrp.jinghuilouyu.cn

PHP:  json_decode($body, true);
来源：http://nrb.hcnkem.com

JS:   await resp.json()
来源：http://omr.feifeiyinyue.top

TS:   await resp.json()
来源：http://jiy.feifeiyinyue.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eky.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pns.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://gbe.ivvv.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lvy.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://tdc.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lte.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hse.fzhhl.top

JS:   resp.ok;  resp.status
来源：http://gbx.jianghu66.top

TS:   resp.ok;  resp.status
来源：http://yqb.yj20258.top

Java: resp.statusCode()
来源：http://amm.svipenyu.cn

Go:   resp.StatusCode
来源：http://zzm.guannengcc.top

Ruby: resp.code.to_i
来源：http://puu.hywenlv.cn

C#:   (int)resp.StatusCode
来源：http://feo.jlsjyb.cn

[L08] 并发请求多个地址
来源：http://llb.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fex.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://slq.sweek.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pff.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qcu.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gwe.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jgf.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qqy.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yak.cashguo.top

================================================================================
来源：http://hdn.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://mns.sysykeji.top


<!-- 参考信息 -->