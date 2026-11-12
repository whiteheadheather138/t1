代发 wailian999

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qcz.gogol.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pyi.yangfankeji.com

[I04] 正则替换
来源：http://pvj.haohaochexian.top

Py:   re.sub(r"\d+", "#", s)
来源：http://ppc.zhaomingkeji.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zqf.daxiang520.top

JS:   s.replace(/\d+/g, "#")
来源：http://rxf.ywan-chungtsiang.top

TS:   s.replace(/\d+/g, "#")
来源：http://vxs.yvedp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ypl.haohaochexian.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jie.ctjpmb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://hgh.ydzc1.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nyd.fehbvm.com

[I05] 按正则拆分
来源：http://nmv.jlsjyb.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rmo.tarul.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jfl.gzhubu.top

JS:   s.split(/\s*,\s*/)
来源：http://uvd.guowangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://ggh.zdqjudy.top

Java: s.split("\\s*,\\s*")
来源：http://vjs.yueranfly.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ibg.cucudq.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sll.c1oappe.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gxs.daxiang520.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mff.daxiang520.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mkn.hywenlv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zrv.bjfxy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://khq.daxiang520.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vgu.smart0.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gap.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bkz.fehbvm.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ana.zdqjudy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eug.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://gni.zdbjq.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://asp.jinyuanbaomall.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://aat.wangdashe.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vzw.jianghu66.top

TS:   /error/gim
来源：http://uzq.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qjf.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wmm.yj20258888.top

Ruby: s.scan(/error/i)
来源：http://pjd.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://khw.xingfuxueyuan.xyz

[I08] 贪婪与非贪婪匹配
来源：http://ybo.vehdjk.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cii.vqdsnc.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://iif.tian-w.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://boq.nwbrower.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qlx.quarkkingdee.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://knx.shanyushiyangtech.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cpp.zhoulong.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyf.vqdsnc.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bjd.zhoulong.xyz

================================================================================
来源：http://awg.tian-w.cn

J. 日期与时间
来源：http://oqn.shangyingyoupin.top

================================================================================
来源：http://srz.tian-w.cn

[J01] 获取当前时间
来源：http://hlt.jlsjyb.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yax.bbcook.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tlw.hammf.cn

JS:   new Date();  Date.now()
来源：http://mix.zhixingplan.top

TS:   new Date();  Date.now()
来源：http://pfj.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uft.cdnleiting.top

Go:   time.Now()
来源：http://atr.hesvh.cn

Ruby: Time.now
来源：http://zew.chenzaomai.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://brl.fzhhl.top

[J02] 格式化输出
来源：http://phb.chenzaomai.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://meq.tian-w.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://snj.yfazqb.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ymu.xuanzx.com

TS:   d.toISOString()
来源：http://vjf.9152youxi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yta.xuanzx.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kmk.yuxming.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jsi.aizwys.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rqq.gzhubu.top

[J03] 字符串解析为日期
来源：http://phk.cucudq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pdp.cqqwz.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pae.bjfxy.top

JS:   new Date("2024-01-02")
来源：http://xyr.sweek.top

TS:   new Date("2024-01-02")
来源：http://rtf.xziqi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fur.hywenlv.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vhp.tianlin.xyz

Ruby: Date.parse("2024-01-02")
来源：http://cus.xylfe.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uuh.quarkkingdee.top

[J04] 时间戳与日期互转
来源：http://sdp.shangyingyoupin.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nub.zhiwuduotai.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hsb.cheryme.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nll.zhoulong.xyz

TS:   Math.floor(Date.now() / 1000)
来源：http://znx.c1oappe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aip.fktsv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nzh.shzxlz.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://umv.ybcxt.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://gkz.shanyushiyangkeji.top

[J05] 时间加减（加 7 天）
来源：http://lro.nanxinkj.top

Py:   now + timedelta(days=7)
来源：http://eqb.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://che.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vgh.yj20258.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://crg.fzhhl.top

Java: LocalDate.now().plusDays(7)
来源：http://hfn.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lgx.cheryme.top

Ruby: Time.now + 7 * 86400
来源：http://qly.fengsongda.top

C#:   DateTime.Now.AddDays(7)
来源：http://ltb.cdnleiting.top

[J06] 计算两时间之差
来源：http://bet.shanyushiyangkeji.top

Py:   (end - start).total_seconds()
来源：http://xzw.tian-w.cn

PHP:  $end->diff($start)->days;
来源：http://qqz.fktsv.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gyl.hesvh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ndy.zhiwuduotai.top

Java: Duration.between(start, end).toSeconds()
来源：http://ebb.xylfe.cn

Go:   end.Sub(start).Hours()
来源：http://ykr.hcnkem.com

Ruby: end - start                 # 返回秒数
来源：http://cel.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://lvb.sweek.top

[J07] 比较两个日期
来源：http://fxc.nanxinkj.top

Py:   d1 < d2;  d1 == d2
来源：http://wat.tanke756.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://onj.nwbrower.top

JS:   d1.getTime() < d2.getTime()
来源：http://ezj.snrcjt.cn

TS:   d1.getTime() < d2.getTime()
来源：http://htr.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://htz.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jwq.yj20258888.top

Ruby: d1 < d2;  d1 == d2
来源：http://bmn.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://fpt.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://wyo.uphjek.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bbt.gogol.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tcy.hesvh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://pih.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uxh.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bku.xuetiantiany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rjb.birdmap.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qom.jinqigufen.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qhh.yangfankeji.com

[J09] 时区处理
来源：http://lgz.hnxiangtu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mqu.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nxc.sweek.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eyi.yfazqb.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://msf.quarkkingdee.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xkp.shanyushiyangkeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pev.ydjk.org.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hcn.shuidangran.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gdl.epnwcf.com

[J10] 取今天 / 本月第一天
来源：http://ybe.fktsv.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rvz.shangyingyoupin.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://snm.jinghuilouyu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ftg.shzxlz.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://goc.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xah.0kj1m.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jxf.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zgg.shanyushiyangtech.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uja.yvedp.cn

================================================================================
来源：http://fvv.tarul.cn

K. JSON 与序列化
来源：http://uch.nwbrower.top

================================================================================
来源：http://rcy.ydjk.org.cn

[K01] 对象转 JSON 字符串
来源：http://qca.birdmap.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iwf.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kwi.daria6918.cn

JS:   JSON.stringify(obj)
来源：http://jfd.xuetiantiany.cn

TS:   JSON.stringify(obj)
来源：http://ocd.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wwp.vehdjk.com

Go:   json.Marshal(obj)
来源：http://vrr.zhoulong.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://yce.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fpb.jiagoushi.top

[K02] JSON 字符串转对象
来源：http://nfn.vehdjk.com

Py:   json.loads(s)
来源：http://dnw.ppjwa.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ooo.haohaochexian.top

JS:   JSON.parse(s)
来源：http://sax.hongshengwenyu.top

TS:   JSON.parse(s)
来源：http://wjr.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://phb.gogol.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://kek.sxryk.cn

Ruby: JSON.parse(s)
来源：http://vzi.yonumen.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qud.zhaomingkeji.xyz

[K03] JSON 美化输出（带缩进）
来源：http://cxp.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wxe.dianchejie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hcs.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ncy.shangyingyoupin.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mre.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bms.zycfv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rej.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://lzh.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hwo.cashguo.top

[K04] 读取 JSON 文件
来源：http://bkc.yj20258.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vsg.quarkkingdee.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://raz.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pex.vqdsnc.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://emq.bbcook.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yfx.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hoe.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://vql.feifeiyinyue.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://iae.svipenyu.cn

[K05] 深拷贝对象
来源：http://mjt.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://lrp.gaohongyu789.top

PHP:  unserialize(serialize($obj));
来源：http://trw.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://lzj.zdbjq.cn

TS:   structuredClone(obj)
来源：http://qsm.jinqigufen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ryo.hfpthk.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://uxa.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tta.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://npc.c1oappe.top

[K06] 解析 URL 查询串
来源：http://wtf.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bhm.feifeiyinyue.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pro.shzxlz.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxx.yuanzhike.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yqg.yj202588.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://shf.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rrv.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tqp.cheryme.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rvb.fktsv.cn

[K07] 进制转换
来源：http://sjo.ydjk.org.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wzz.xinyue.icu

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gzk.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qqa.9152youxi.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://llo.316326.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wtn.jlsjyb.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qzb.hammf.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cnj.cashguo.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gav.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://ics.yj202588.top

Py:   pickle.dumps(obj)
来源：http://kca.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://glp.ctjpmb.com

JS:   v8.serialize(obj)        // Node
来源：http://bii.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ggs.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kqq.zycfv.cn

Go:   encoding/gob
来源：http://qhw.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://hyq.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ehl.9152youxi.cn

================================================================================
来源：http://rfi.fanxiaobao.xyz

L. 网络请求
来源：http://lqh.xziqi.cn

================================================================================
来源：http://yhl.jyoumei.cn

[L01] 发送 GET 请求
来源：http://okv.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zhg.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://voo.ppjwa.cn

JS:   await fetch(url)
来源：http://qsk.hfpthk.cn

TS:   await fetch(url)
来源：http://ujn.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rra.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://ctc.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://sgp.yj20258888.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tud.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://hgl.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wfm.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wao.nanxuanxn.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hnu.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ttc.nanxuanxn.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wku.tanke756.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qkx.hnqzz.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gwo.snrcjt.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dsg.xuetiantiany.cn

[L03] 设置自定义请求头
来源：http://hei.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gyn.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://idr.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kxl.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://grk.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://lrs.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uie.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://atp.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ssl.chenzaomai.com

[L04] 设置超时
来源：http://ozf.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://xlg.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wwi.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xal.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aen.xuetiantiany.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lei.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hki.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://egw.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bau.gzhubu.top

[L05] 上传文件（multipart）
来源：http://axm.yonumen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kwb.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sim.vehdjk.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cfx.xinyue.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qul.hcnkem.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vrb.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rtj.zhaomingkeji.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://yud.xingfuxueyuan.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://smn.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://hbg.hammf.cn

Py:   resp.json()
来源：http://rxa.quarkkingdee.top

PHP:  json_decode($body, true);
来源：http://gtr.fzhhl.top

JS:   await resp.json()
来源：http://mrd.chenzaomai.com

TS:   await resp.json()
来源：http://jlr.nanxinkj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://qrd.nanxinkj.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://acn.cheryme.top

Ruby: JSON.parse(resp.body)
来源：http://keg.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uyb.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://fvu.uphjek.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nrz.yuxming.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ztb.zdqjudy.top

JS:   resp.ok;  resp.status
来源：http://abz.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://zji.feifeiyinyue.top

Java: resp.statusCode()
来源：http://knx.jiagoushi.top

Go:   resp.StatusCode
来源：http://cjm.sweek.top

Ruby: resp.code.to_i
来源：http://ysi.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://mye.shzxlz.cn

[L08] 并发请求多个地址
来源：http://fyx.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ihx.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://ykq.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ufk.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ezd.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mlc.dashuyun.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dif.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jwz.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ylj.jiagoushi.top

================================================================================
来源：http://uep.52xcode.cn

M. 命令行 / 进程 / 环境
来源：http://xyr.wangshuangyany.cn

================================================================================
来源：http://ego.316326.xyz

[M01] 读取命令行参数
来源：http://fzt.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://adq.shanyushiyangkeji.top

PHP:  $argv;  $argc;
来源：http://ttq.yangfankeji.com

JS:   process.argv.slice(2)
来源：http://bcq.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://uxi.xinyue.icu

Java: args 数组（main 方法参数）
来源：http://bec.jyoumei.cn

Go:   os.Args[1:]
来源：http://fgj.yueranfly.top


<!-- 参考信息 -->