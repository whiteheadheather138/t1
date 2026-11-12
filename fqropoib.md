代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://gxv.wangshuangyany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sqo.ywan-chungtsiang.top

JS:   s.split(/\s*,\s*/)
来源：http://qus.fzhhl.top

TS:   s.split(/\s*,\s*/)
来源：http://fcm.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://xeu.bjfxy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kmt.xylfe.cn

Ruby: s.split(/\s*,\s*/)
来源：http://eyq.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tuc.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jga.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zbi.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lgg.bbcook.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qqp.wangdashe.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ukz.shanyushiyangtech.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bmz.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://azm.hfpthk.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xol.dashuyun.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pnv.daria6918.cn

[I07] 忽略大小写与多行模式
来源：http://boq.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://byw.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xti.haohaochexian.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kba.sufxvd.cn

TS:   /error/gim
来源：http://tii.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ygh.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wud.jinqigufen.top

Ruby: s.scan(/error/i)
来源：http://pot.sweek.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://teb.ctjpmb.com

[I08] 贪婪与非贪婪匹配
来源：http://vbd.zhongyouzk.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vjw.feifeiyinyue.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uof.xuetiantiany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lgw.meibo888.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sti.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://vzn.zhiwuduotai.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fdw.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uys.shanyushiyangtech.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ipk.aibaodan.cn

================================================================================
来源：http://zyh.9152youxi.cn

J. 日期与时间
来源：http://cik.nwbrower.top

================================================================================
来源：http://zjb.dashuyun.cn

[J01] 获取当前时间
来源：http://elg.ctjpmb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ckc.shangyingyoupin.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://okj.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://izb.chenjidiqi.icu

TS:   new Date();  Date.now()
来源：http://ffj.gogol.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uzk.jinyuanbaomall.cn

Go:   time.Now()
来源：http://wkj.xuanzx.com

Ruby: Time.now
来源：http://nkb.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ipf.cheryme.top

[J02] 格式化输出
来源：http://upo.yuxming.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uqg.cdnleiting.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://aeq.nanxinkj.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tuc.hysaishi.cn

TS:   d.toISOString()
来源：http://edn.bjfxy.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mvp.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vxs.sufxvd.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ouz.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wcy.zdbjq.cn

[J03] 字符串解析为日期
来源：http://dvy.xuetiantiany.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bai.jianghu66.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qac.sysykeji.top

JS:   new Date("2024-01-02")
来源：http://bwf.shangyingyoupin.top

TS:   new Date("2024-01-02")
来源：http://raz.daxiang520.top

Java: LocalDate.parse("2024-01-02")
来源：http://rza.ydzc1.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ivn.jinghuilouyu.cn

Ruby: Date.parse("2024-01-02")
来源：http://qcc.guowangkeji.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oqf.xylfe.cn

[J04] 时间戳与日期互转
来源：http://vpk.aibaodan.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qsa.sweek.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zoz.sjlbkw.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jyc.gzhubu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://vyn.cqqwz.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zot.jianghu66.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hyh.c1oappe.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://trt.fktsv.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fru.vqdsnc.cn

[J05] 时间加减（加 7 天）
来源：http://tla.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://imo.shanyushiyangtech.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ofk.tarul.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vcu.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eiw.quarkkingdee.top

Java: LocalDate.now().plusDays(7)
来源：http://nqk.bbcook.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mtw.zhongyouzk.top

Ruby: Time.now + 7 * 86400
来源：http://fxf.bbcook.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rlw.xuetiantiany.cn

[J06] 计算两时间之差
来源：http://wxm.ehwqpu.com

Py:   (end - start).total_seconds()
来源：http://frb.yvedp.cn

PHP:  $end->diff($start)->days;
来源：http://vvx.fehbvm.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cgx.shanyushiyangkeji.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rkh.ywan-chungtsiang.top

Java: Duration.between(start, end).toSeconds()
来源：http://oyx.andypj.xyz

Go:   end.Sub(start).Hours()
来源：http://esb.wangshuangyany.cn

Ruby: end - start                 # 返回秒数
来源：http://vrx.zdbjq.cn

C#:   (end - start).TotalSeconds
来源：http://cgg.tianlin.xyz

[J07] 比较两个日期
来源：http://gbo.havefunace.top

Py:   d1 < d2;  d1 == d2
来源：http://yjq.ivvv.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ifq.sweek.top

JS:   d1.getTime() < d2.getTime()
来源：http://zvf.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://aba.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vrz.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ovj.redwolf501.top

Ruby: d1 < d2;  d1 == d2
来源：http://kxu.fengsongda.top

C#:   d1 < d2;  d1 == d2
来源：http://yrg.tarul.cn

[J08] 提取年月日与星期
来源：http://byc.yongpay.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vjz.xziqi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hwy.hfpthk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jxu.aibaodan.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zok.yanxiufei.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wmj.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ugo.yj20258.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vyq.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aqy.xziqi.cn

[J09] 时区处理
来源：http://tnz.jinghuilouyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bwd.iojbl.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nle.jiagoushi.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dok.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kyy.ybcxt.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://umy.shanyushiyangtech.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tkh.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bkw.hcnkem.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tsd.gaohongyu789.top

[J10] 取今天 / 本月第一天
来源：http://wsu.smart0.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://voh.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://aqv.wangdashe.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sxu.xziqi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uce.guannengcc.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egh.shuidangran.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kuj.cheryme.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jzw.ybcxt.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://emk.aibaodan.cn

================================================================================
来源：http://pml.hnxiangtu.top

K. JSON 与序列化
来源：http://nbr.gogol.net.cn

================================================================================
来源：http://sdp.sweek.top

[K01] 对象转 JSON 字符串
来源：http://pxl.hammf.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yly.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gdg.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://fby.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://wgf.fanxiaobao.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://glp.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://qpk.zhengqikj.top

Ruby: obj.to_json                                     // require "json"
来源：http://wxk.xziqi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bzt.tian-w.cn

[K02] JSON 字符串转对象
来源：http://vfq.hnxiangtu.top

Py:   json.loads(s)
来源：http://npn.xinyue.icu

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rpg.kuanghao11.cn

JS:   JSON.parse(s)
来源：http://ygb.gaohongyu789.top

TS:   JSON.parse(s)
来源：http://asc.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bah.gaohongyu789.top

Go:   json.Unmarshal(data, &v)
来源：http://prp.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://moa.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zyw.smart0.xyz

[K03] JSON 美化输出（带缩进）
来源：http://pkn.dianchejie.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gwr.zycfv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mfq.hfpthk.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sqn.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://xby.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zqv.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rdp.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://ygk.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://een.cdnleiting.top

[K04] 读取 JSON 文件
来源：http://gtb.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tpz.fktsv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zud.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wuh.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ibg.yfazqb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wlb.ctjpmb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://esu.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://kbv.9152youxi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ypb.fehbvm.com

[K05] 深拷贝对象
来源：http://ssf.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://rya.uphjek.com

PHP:  unserialize(serialize($obj));
来源：http://ukg.52xcode.cn

JS:   structuredClone(obj)
来源：http://lyu.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://hba.cheryme.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mgc.chenlongwang.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cwm.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dyf.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wll.mhx1999.top

[K06] 解析 URL 查询串
来源：http://hik.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ivi.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xxx.quarkkingdee.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://utj.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zdn.zhijiandao.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://nqs.c1oappe.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lvi.zhongyouzk.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hik.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jum.mhx1999.top

[K07] 进制转换
来源：http://rao.ctjpmb.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ell.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tni.9152youxi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ljo.aizwys.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vpo.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ngx.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vfd.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rae.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bgi.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://nwd.hongshengwenyu.top

Py:   pickle.dumps(obj)
来源：http://mwq.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ath.aizwys.cn

JS:   v8.serialize(obj)        // Node
来源：http://rqb.chenzaomai.com

TS:   v8.serialize(obj)        // Node
来源：http://abs.cdnleiting.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hpl.yj20258.top

Go:   encoding/gob
来源：http://tdo.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://txp.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jwr.0kj1m.cn

================================================================================
来源：http://ejw.52xcode.cn

L. 网络请求
来源：http://get.zycfv.cn

================================================================================
来源：http://kwy.jqgfzy.top

[L01] 发送 GET 请求
来源：http://fyx.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hkj.jyoumei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://olv.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://vto.hcnkem.com

TS:   await fetch(url)
来源：http://vqd.yonumen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rod.gogol.net.cn

Go:   resp, err := http.Get(url)
来源：http://pup.hongshengwenyu.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dzl.xinyue.icu

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jux.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://yjy.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://inc.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nhm.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rsn.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wby.zhixingplan.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yjj.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oog.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ehg.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gzs.ydzc1.top

[L03] 设置自定义请求头
来源：http://bkh.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mgf.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ndp.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dfo.tian-w.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wou.hysaishi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://syk.ehwqpu.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hba.quarkkingdee.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ths.vehdjk.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xbt.yueranfly.top

[L04] 设置超时
来源：http://hsg.tanke756.top

Py:   requests.get(url, timeout=5)
来源：http://xiv.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rlz.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bka.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tui.zhengqikj.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qdz.hysaishi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xcv.9152youxi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://qku.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fip.zhijiandao.cn

[L05] 上传文件（multipart）
来源：http://kvx.hysaishi.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tnk.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mwe.sxryk.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yaa.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bgx.fktsv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tjz.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xkl.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mbe.yfazqb.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dcz.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://kjx.yj20258.top

Py:   resp.json()
来源：http://pcw.xingfuxueyuan.xyz

PHP:  json_decode($body, true);
来源：http://qel.52xcode.cn

JS:   await resp.json()
来源：http://ncc.daxiang520.top

TS:   await resp.json()
来源：http://pxm.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dwp.jiagoushi.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://arv.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://iog.cqqwz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jfp.dashuyun.cn

[L07] 处理 HTTP 状态码
来源：http://yhl.andypj.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oxq.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tqu.havefunace.top

JS:   resp.ok;  resp.status
来源：http://crd.jqgufenzy.top

TS:   resp.ok;  resp.status
来源：http://zhp.jqgufenzy.top

Java: resp.statusCode()
来源：http://bhv.yj202588.top

Go:   resp.StatusCode
来源：http://rri.ehwqpu.com

Ruby: resp.code.to_i
来源：http://zws.jiagoushi.top

C#:   (int)resp.StatusCode
来源：http://kfp.gzhubu.top

[L08] 并发请求多个地址
来源：http://tya.zhixingplan.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lwu.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://kmd.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ucd.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nhc.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://eqo.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dtg.birdmap.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mdc.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xyx.zdbjq.cn

================================================================================
来源：http://udw.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://qda.havefunace.top

================================================================================
来源：http://qmm.yongpay.top

[M01] 读取命令行参数
来源：http://xbz.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://zea.bjfxy.top

PHP:  $argv;  $argc;
来源：http://hvr.hesvh.cn

JS:   process.argv.slice(2)
来源：http://fuk.wangshuangyany.cn

TS:   process.argv.slice(2)
来源：http://wpp.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://gmm.ehwqpu.com

Go:   os.Args[1:]
来源：http://ybj.hesvh.cn

Ruby: ARGV
来源：http://zlb.yonumen.top

C#:   args 数组（Main 方法参数）
来源：http://gqe.yj202588.top

[M02] 读取环境变量
来源：http://cyw.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://sih.yj20258.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://itn.aizwys.cn

JS:   process.env.HOME
来源：http://huj.iojbl.cn

TS:   process.env.HOME
来源：http://cos.wangshuangyany.cn

Java: System.getenv("HOME")
来源：http://bsg.ybcxt.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rtl.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://bib.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nnz.fktsv.cn

[M03] 执行外部命令
来源：http://dic.hysaishi.cn


<!-- 参考信息 -->