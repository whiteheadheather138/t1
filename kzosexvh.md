代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://qkf.meibo888.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sdw.chenzaomai.com

JS:   s.split(/\s*,\s*/)
来源：http://cpd.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://rcs.chenlongwang.top

Java: s.split("\\s*,\\s*")
来源：http://dct.xuetiantiany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bid.zdqjudy.top

Ruby: s.split(/\s*,\s*/)
来源：http://ajl.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lyd.shanyushiyangkeji.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wea.0kj1m.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wdl.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vyd.pycfn.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://luw.zhixingplan.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wuw.tarul.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rup.ctjpmb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vfq.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ndx.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bkj.smart0.xyz

[I07] 忽略大小写与多行模式
来源：http://azm.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uxx.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gwh.zhixingplan.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xrp.c1oappe.top

TS:   /error/gim
来源：http://glg.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ytn.ydzc1.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wme.wangdashe.top

Ruby: s.scan(/error/i)
来源：http://xlo.zhijiandao.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://flf.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://vvq.quarkkingdee.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hou.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vgw.cashguo.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rms.sweek.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qet.daria6918.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cqa.52xcode.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gwn.0kj1m.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wsz.hfpthk.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ewg.ydzc1.top

================================================================================
来源：http://erz.316326.xyz

J. 日期与时间
来源：http://lsw.vehdjk.com

================================================================================
来源：http://wbx.tian-w.cn

[J01] 获取当前时间
来源：http://zto.pycfn.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qto.hongshengwenyu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jjd.vehdjk.com

JS:   new Date();  Date.now()
来源：http://myi.shuidangran.top

TS:   new Date();  Date.now()
来源：http://fsj.nwbrower.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mco.shuidangran.top

Go:   time.Now()
来源：http://vdj.fktsv.cn

Ruby: Time.now
来源：http://ieg.xziqi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vxw.xylfe.cn

[J02] 格式化输出
来源：http://anc.fzhhl.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wqy.guowangkeji.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dbs.yonumen.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://aea.aizwys.cn

TS:   d.toISOString()
来源：http://jdd.gaohongyu789.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://eke.gogol.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vqu.cheryme.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://its.xylfe.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://syo.xingfuxueyuan.xyz

[J03] 字符串解析为日期
来源：http://hgc.zdbjq.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xzk.ivvv.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rvi.andypj.xyz

JS:   new Date("2024-01-02")
来源：http://tna.hnxiangtu.top

TS:   new Date("2024-01-02")
来源：http://ief.dianchejie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tvo.xuetiantiany.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mro.vqdsnc.cn

Ruby: Date.parse("2024-01-02")
来源：http://uja.yueranfly.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tdi.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://nmh.guowangkeji.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mvs.cashguo.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wqg.daxiang520.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xqx.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://ygn.nwbrower.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://enc.gaohongyu789.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gox.fehbvm.com

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zyx.shanyushiyangtech.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://czl.xziqi.cn

[J05] 时间加减（加 7 天）
来源：http://bxu.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://ppc.yj202588.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://epr.sxryk.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://etq.kuanghao11.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fes.yj20258888.top

Java: LocalDate.now().plusDays(7)
来源：http://hun.sxryk.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kgg.zhiwuduotai.top

Ruby: Time.now + 7 * 86400
来源：http://xxq.hesvh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zmv.hesvh.cn

[J06] 计算两时间之差
来源：http://sud.yj20258.top

Py:   (end - start).total_seconds()
来源：http://frm.cashguo.top

PHP:  $end->diff($start)->days;
来源：http://sjz.bjfxy.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zem.zhaomingkeji.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vho.aibaodan.cn

Java: Duration.between(start, end).toSeconds()
来源：http://pyf.pycfn.com

Go:   end.Sub(start).Hours()
来源：http://gtz.mhx1999.top

Ruby: end - start                 # 返回秒数
来源：http://myw.shanyushiyangkeji.top

C#:   (end - start).TotalSeconds
来源：http://vao.chenlongwang.top

[J07] 比较两个日期
来源：http://eou.jqgufenzy.top

Py:   d1 < d2;  d1 == d2
来源：http://kyb.smart0.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yye.vqdsnc.cn

JS:   d1.getTime() < d2.getTime()
来源：http://wqf.yueranfly.top

TS:   d1.getTime() < d2.getTime()
来源：http://mtv.yj20258888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fjj.jyoumei.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hfk.ywan-chungtsiang.top

Ruby: d1 < d2;  d1 == d2
来源：http://euw.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://zna.zhixingplan.top

[J08] 提取年月日与星期
来源：http://jdx.gzhubu.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wxl.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qec.fehbvm.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tnd.hcnkem.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jxx.gaohongyu789.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sjb.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wkb.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cag.hnxiangtu.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hig.tianlin.xyz

[J09] 时区处理
来源：http://sxh.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ufz.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://syr.yj20258.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ory.nwbrower.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yot.hysaishi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jlo.ppjwa.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tdn.316326.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://qce.jinghuilouyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fxl.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://jgl.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://spe.ywan-chungtsiang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eil.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qnm.tianlin.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qbm.smart0.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://agc.birdmap.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xeu.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cbs.fengsongda.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://htc.fanxiaobao.xyz

================================================================================
来源：http://hnj.xuetiantiany.cn

K. JSON 与序列化
来源：http://lme.pycfn.com

================================================================================
来源：http://nfv.zhijiandao.cn

[K01] 对象转 JSON 字符串
来源：http://lhw.tian-w.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://otc.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zdu.316326.xyz

JS:   JSON.stringify(obj)
来源：http://xoz.redwolf501.top

TS:   JSON.stringify(obj)
来源：http://rqg.bbcook.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zgw.jyoumei.cn

Go:   json.Marshal(obj)
来源：http://tuk.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://bec.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bjd.cqqwz.cn

[K02] JSON 字符串转对象
来源：http://dqp.smart0.xyz

Py:   json.loads(s)
来源：http://qsx.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yfw.wangdashe.top

JS:   JSON.parse(s)
来源：http://gee.bbcook.cn

TS:   JSON.parse(s)
来源：http://ycl.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xxh.birdmap.top

Go:   json.Unmarshal(data, &v)
来源：http://vli.jyoumei.cn

Ruby: JSON.parse(s)
来源：http://ubx.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zlr.shanyushiyangtech.top

[K03] JSON 美化输出（带缩进）
来源：http://gff.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://srp.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zyx.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cjt.ctjpmb.com

TS:   JSON.stringify(obj, null, 2)
来源：http://riw.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kbt.vehdjk.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ogh.yuanzhike.top

Ruby: JSON.pretty_generate(obj)
来源：http://wqt.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dkn.xinyue.icu

[K04] 读取 JSON 文件
来源：http://umf.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yfd.guannengcc.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hfo.chenlongwang.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ypv.hywenlv.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://atg.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rqq.pengpengdd.cyou

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lpr.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jnv.yj20258.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kdz.shuidangran.top

[K05] 深拷贝对象
来源：http://xwa.ydjk.org.cn

Py:   copy.deepcopy(obj)
来源：http://yuq.tian-w.cn

PHP:  unserialize(serialize($obj));
来源：http://vtr.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://wbe.bbcook.cn

TS:   structuredClone(obj)
来源：http://dkh.xuetiantiany.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://spr.vehdjk.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bmj.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bvr.yanxiufei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://adx.jinqigufen.top

[K06] 解析 URL 查询串
来源：http://bdi.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xnm.jianghu66.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xny.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rze.guowangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyv.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gxz.sufxvd.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://ksg.epnwcf.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kyz.yueranfly.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wwi.zhiwuduotai.top

[K07] 进制转换
来源：http://akc.52xcode.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qkx.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nig.fktsv.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zby.nanxinkj.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqj.bbcook.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ksh.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://obo.wangdashe.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lyr.ctjpmb.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vya.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://nrh.yuanzhike.top

Py:   pickle.dumps(obj)
来源：http://sak.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://cbb.shuidangran.top

JS:   v8.serialize(obj)        // Node
来源：http://qpx.hammf.cn

TS:   v8.serialize(obj)        // Node
来源：http://bks.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://foh.sysykeji.top

Go:   encoding/gob
来源：http://luh.zhaomingkeji.xyz

Ruby: Marshal.dump(obj)
来源：http://fad.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://yta.52xcode.cn

================================================================================
来源：http://fgs.tarul.cn

L. 网络请求
来源：http://alh.mhx1999.top

================================================================================
来源：http://gau.xuetiantiany.cn

[L01] 发送 GET 请求
来源：http://szy.zycfv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wrp.chenjidiqi.icu

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gwr.xinyue.icu

JS:   await fetch(url)
来源：http://pfy.cashguo.top

TS:   await fetch(url)
来源：http://zbe.c1oappe.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sfv.sysykeji.top

Go:   resp, err := http.Get(url)
来源：http://uqp.ctjpmb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rgj.xziqi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ari.tarul.cn

[L02] 发送 POST JSON
来源：http://qwh.shanyushiyangkeji.top

Py:   requests.post(url, json={"a": 1})
来源：http://kct.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vqi.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qlm.yueranfly.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://igo.zhoulong.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qjy.ivvv.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://juo.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://skv.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bmy.gotoacloud.top

[L03] 设置自定义请求头
来源：http://lqs.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tjc.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://rni.zhongyouzk.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zfo.0kj1m.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vqt.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nch.fzhhl.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zti.jqgfzy.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cud.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lto.sjlbkw.cn

[L04] 设置超时
来源：http://rqs.yuxming.cn

Py:   requests.get(url, timeout=5)
来源：http://upa.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mlf.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ley.meibo888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vat.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ymx.mhx1999.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wvo.jinqigufen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hsw.yvedp.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://epl.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://fcd.fktsv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bvz.yueranfly.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vgv.gotoacloud.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ftx.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bmr.52xcode.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://std.pengpengdd.cyou

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://gno.cqqwz.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hdd.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://swm.ivvv.top

[L06] 解析响应为 JSON
来源：http://xdw.zhoulong.xyz

Py:   resp.json()
来源：http://fmg.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://peq.shzxlz.cn

JS:   await resp.json()
来源：http://pxh.havefunace.top

TS:   await resp.json()
来源：http://xtg.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zvl.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zxn.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://hux.snrcjt.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ddl.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://mst.jinqigufen.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://foa.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://onm.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://cyt.yj20258888.top

TS:   resp.ok;  resp.status
来源：http://acq.cdnleiting.top

Java: resp.statusCode()
来源：http://npx.xinyue.icu

Go:   resp.StatusCode
来源：http://jko.yj20258.top

Ruby: resp.code.to_i
来源：http://zkc.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://zcr.zdqjudy.top

[L08] 并发请求多个地址
来源：http://cfy.kuanghao11.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qlg.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://hwy.yj20258.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dzd.jinqigufen.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xut.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qyi.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pfc.zhixingplan.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://yxr.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fty.guannengcc.top

================================================================================
来源：http://cfw.cucudq.cn

M. 命令行 / 进程 / 环境
来源：http://yhy.vqdsnc.cn

================================================================================
来源：http://guq.vqdsnc.cn

[M01] 读取命令行参数
来源：http://trl.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://sft.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://chh.52xcode.cn

JS:   process.argv.slice(2)
来源：http://ldx.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://bpd.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://gyx.dashuyun.cn

Go:   os.Args[1:]
来源：http://psa.snrcjt.cn

Ruby: ARGV
来源：http://hul.zdqjudy.top

C#:   args 数组（Main 方法参数）
来源：http://fri.yuxming.cn

[M02] 读取环境变量
来源：http://rlo.guowangkeji.top

Py:   os.environ.get("HOME")
来源：http://oiu.fengsongda.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cgy.mhx1999.top

JS:   process.env.HOME
来源：http://lbs.tanke756.top

TS:   process.env.HOME
来源：http://ocv.c1oappe.top

Java: System.getenv("HOME")
来源：http://oot.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://sqk.hcnkem.com

Ruby: ENV["HOME"]
来源：http://zyc.hysaishi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qxx.sxryk.cn

[M03] 执行外部命令
来源：http://mmg.nanxinkj.top


<!-- 参考信息 -->