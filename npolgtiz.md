代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://gjt.dashuyun.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lby.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://sdb.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://ovb.gaohongyu789.top

Java: s.split("\\s*,\\s*")
来源：http://viw.yuxming.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jjk.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://ldz.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zzf.haohaochexian.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://etm.zhixingplan.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://urw.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://skq.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ucj.yongpay.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gal.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dzq.hysaishi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ucb.fktsv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mag.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ylx.pengpengdd.cyou

[I07] 忽略大小写与多行模式
来源：http://ywk.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mxs.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jhy.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wvi.zhoulong.xyz

TS:   /error/gim
来源：http://gun.havefunace.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qvc.guannengcc.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kca.gzhubu.top

Ruby: s.scan(/error/i)
来源：http://buj.dashuyun.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ymh.jqgufenzy.top

[I08] 贪婪与非贪婪匹配
来源：http://qkq.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bll.mhx1999.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mke.shangyingyoupin.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://alv.dianchejie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lkj.hammf.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ehk.nanxuanxn.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yiw.fanxiaobao.xyz

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://srz.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gqx.hongshengwenyu.top

================================================================================
来源：http://urk.jinyuanbaomall.cn

J. 日期与时间
来源：http://ipz.zhijiandao.cn

================================================================================
来源：http://jws.jqgufenzy.top

[J01] 获取当前时间
来源：http://sgv.jqgufenzy.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://ezc.zhixingplan.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eup.zhoulong.xyz

JS:   new Date();  Date.now()
来源：http://vwd.wangdashe.top

TS:   new Date();  Date.now()
来源：http://pxr.cdnleiting.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mon.daria6918.cn

Go:   time.Now()
来源：http://tph.havefunace.top

Ruby: Time.now
来源：http://plq.feifeiyinyue.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gpt.xinyue.icu

[J02] 格式化输出
来源：http://auj.jyoumei.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dlr.fktsv.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ovu.hammf.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cch.hcnkem.com

TS:   d.toISOString()
来源：http://oou.hysaishi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fbd.fzhhl.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vxc.yfazqb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jpx.xuetiantiany.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aft.sxryk.cn

[J03] 字符串解析为日期
来源：http://uxn.ivvv.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xdz.aizwys.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://akm.hnxiangtu.top

JS:   new Date("2024-01-02")
来源：http://fgg.ydzc1.top

TS:   new Date("2024-01-02")
来源：http://adb.c1oappe.top

Java: LocalDate.parse("2024-01-02")
来源：http://bju.yfazqb.com

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://npx.zdqjudy.top

Ruby: Date.parse("2024-01-02")
来源：http://ifs.jiagoushi.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ddj.cheryme.top

[J04] 时间戳与日期互转
来源：http://yzs.jyoumei.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rmi.jlsjyb.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ujn.jyoumei.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dws.shangyingyoupin.top

TS:   Math.floor(Date.now() / 1000)
来源：http://nzv.gzhubu.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zro.yj20258.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cwn.aizwys.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://crp.jinqigufen.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jom.ehwqpu.com

[J05] 时间加减（加 7 天）
来源：http://fnf.yangfankeji.com

Py:   now + timedelta(days=7)
来源：http://eoj.guowangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nss.shuidangran.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jdo.shangyingyoupin.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lcq.jqgufenzy.top

Java: LocalDate.now().plusDays(7)
来源：http://eil.yanxiufei.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://euj.ydzc1.top

Ruby: Time.now + 7 * 86400
来源：http://svq.cdnleiting.top

C#:   DateTime.Now.AddDays(7)
来源：http://mdg.feifeiyinyue.top

[J06] 计算两时间之差
来源：http://mwk.yueranfly.top

Py:   (end - start).total_seconds()
来源：http://rfg.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://wog.yongpay.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://czc.tianlin.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kbm.xziqi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://npm.sufxvd.cn

Go:   end.Sub(start).Hours()
来源：http://pph.zhaomingkeji.xyz

Ruby: end - start                 # 返回秒数
来源：http://ysa.shuidangran.top

C#:   (end - start).TotalSeconds
来源：http://csn.yanxiufei.cn

[J07] 比较两个日期
来源：http://tsx.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://cdi.zhongyouzk.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qdh.zhijiandao.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ppb.shzxlz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://msf.birdmap.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mix.gotoacloud.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uyi.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kni.kuanghao11.cn

C#:   d1 < d2;  d1 == d2
来源：http://rig.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://vmp.hysaishi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lwy.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fff.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dea.hfpthk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pno.ehwqpu.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dqt.zycfv.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mxd.zhijiandao.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cks.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://eyd.feifeiyinyue.top

[J09] 时区处理
来源：http://wee.fzhhl.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ixy.gotoacloud.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fgb.yj202588.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xgb.316326.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sez.yj20258888.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ese.aizwys.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://net.zhixingplan.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ffp.iojbl.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gfi.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://oft.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://bdn.jianghu66.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jwe.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kme.yvedp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jpm.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://req.epnwcf.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ebj.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yru.gotoacloud.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://reb.shuidangran.top

================================================================================
来源：http://qhs.yj202588.top

K. JSON 与序列化
来源：http://crl.chenlongwang.top

================================================================================
来源：http://psu.meibo888.top

[K01] 对象转 JSON 字符串
来源：http://mvv.shangyingyoupin.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jxr.jinqigfzy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://okj.hnqzz.top

JS:   JSON.stringify(obj)
来源：http://inm.xinyue.icu

TS:   JSON.stringify(obj)
来源：http://onf.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lts.tanke756.top

Go:   json.Marshal(obj)
来源：http://shr.ywan-chungtsiang.top

Ruby: obj.to_json                                     // require "json"
来源：http://vof.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://wkg.andypj.xyz

[K02] JSON 字符串转对象
来源：http://ati.zycfv.cn

Py:   json.loads(s)
来源：http://sxg.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://icm.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://vvr.ydzc1.top

TS:   JSON.parse(s)
来源：http://iep.meibo888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xhe.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://alk.ydzc1.top

Ruby: JSON.parse(s)
来源：http://lhl.fzhhl.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uov.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://jnx.fzhhl.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dph.shuidangran.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iwy.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://mst.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ygj.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fzp.kuanghao11.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gle.chenzaomai.com

Ruby: JSON.pretty_generate(obj)
来源：http://jfa.xylfe.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vsh.yvedp.cn

[K04] 读取 JSON 文件
来源：http://ebj.andypj.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uvf.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pev.cashguo.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cpp.hnqzz.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sgu.vqdsnc.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cae.yfazqb.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zfq.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tbb.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gwr.ctjpmb.com

[K05] 深拷贝对象
来源：http://ucf.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://mde.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://mea.zhoulong.xyz

JS:   structuredClone(obj)
来源：http://cng.epnwcf.com

TS:   structuredClone(obj)
来源：http://olj.hongshengwenyu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fdx.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nyj.mhx1999.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wgc.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jwu.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://yvl.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wti.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rga.xingfuxueyuan.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mza.zdbjq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qew.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://klw.sjlbkw.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xyc.zhixingplan.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gjw.yonumen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://too.birdmap.top

[K07] 进制转换
来源：http://tmy.zdqjudy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mus.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xkj.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tca.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yel.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yit.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ych.cqqwz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gwe.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nsn.yangfankeji.com

[K08] 二进制序列化（非 JSON）
来源：http://jol.sxryk.cn

Py:   pickle.dumps(obj)
来源：http://qiv.zhongyouzk.top

PHP:  serialize($obj);  unserialize($s);
来源：http://fzr.hysaishi.cn

JS:   v8.serialize(obj)        // Node
来源：http://mvn.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://bdj.tianlin.xyz

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jbm.tianlin.xyz

Go:   encoding/gob
来源：http://pbc.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://jwm.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://iau.316326.xyz

================================================================================
来源：http://rpb.hnxiangtu.top

L. 网络请求
来源：http://srr.fzhhl.top

================================================================================
来源：http://vyc.hcnkem.com

[L01] 发送 GET 请求
来源：http://xxp.yanxiufei.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hth.vqdsnc.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nua.dashuyun.cn

JS:   await fetch(url)
来源：http://jrw.bbcook.cn

TS:   await fetch(url)
来源：http://ssz.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://yey.9152youxi.cn

Go:   resp, err := http.Get(url)
来源：http://rkf.yueranfly.top

Ruby: Net::HTTP.get(URI(url))
来源：http://sfo.hywenlv.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://igx.316326.xyz

[L02] 发送 POST JSON
来源：http://gdt.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://lva.daxiang520.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nqf.andypj.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmh.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kny.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wnj.hongshengwenyu.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cbh.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hfs.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uig.aibaodan.cn

[L03] 设置自定义请求头
来源：http://mvs.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bbj.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://les.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cgj.sweek.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hnw.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://snm.feifeiyinyue.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bma.zhongyouzk.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wlb.yangfankeji.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qda.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://ulz.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://zzh.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://try.hongshengwenyu.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jhu.zycfv.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pyi.jinqigfzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nwt.sweek.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xpd.jqgfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lip.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rlr.zhixingplan.top

[L05] 上传文件（multipart）
来源：http://zpg.ydjk.org.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://opa.zhoulong.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hmk.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cdi.epnwcf.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qxj.zycfv.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ahr.yongpay.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://uhp.shuidangran.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bkb.fengsongda.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://frf.yfazqb.com

[L06] 解析响应为 JSON
来源：http://emu.jinqigufen.top

Py:   resp.json()
来源：http://azb.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://ayn.cqqwz.cn

JS:   await resp.json()
来源：http://wcq.andypj.xyz

TS:   await resp.json()
来源：http://bjl.sufxvd.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dyb.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bnb.hongshengwenyu.top

Ruby: JSON.parse(resp.body)
来源：http://nnb.fktsv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ohs.chenjidiqi.icu

[L07] 处理 HTTP 状态码
来源：http://ssm.xziqi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://frr.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gtz.zhiwuduotai.top

JS:   resp.ok;  resp.status
来源：http://dum.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://rnx.zhijiandao.cn

Java: resp.statusCode()
来源：http://kzu.tarul.cn

Go:   resp.StatusCode
来源：http://npa.gogol.net.cn

Ruby: resp.code.to_i
来源：http://hac.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://fcm.wangdashe.top

[L08] 并发请求多个地址
来源：http://rzx.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qqz.nwbrower.top

PHP:  curl_multi_init() 系列
来源：http://zix.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pby.gaohongyu789.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://amg.zycfv.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mbd.svipenyu.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zig.hesvh.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mlb.hcnkem.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ebs.hongshengwenyu.top

================================================================================
来源：http://tls.hammf.cn

M. 命令行 / 进程 / 环境
来源：http://wda.jqgufenzy.top

================================================================================
来源：http://brw.sysykeji.top

[M01] 读取命令行参数
来源：http://cww.jinyuanbaomall.cn

Py:   sys.argv[1:]
来源：http://ppd.cqqwz.cn

PHP:  $argv;  $argc;
来源：http://ddq.hywenlv.cn

JS:   process.argv.slice(2)
来源：http://umo.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://akm.hammf.cn

Java: args 数组（main 方法参数）
来源：http://fdb.tian-w.cn

Go:   os.Args[1:]
来源：http://iml.bbcook.cn

Ruby: ARGV
来源：http://hon.0kj1m.cn

C#:   args 数组（Main 方法参数）
来源：http://zmg.smart0.xyz

[M02] 读取环境变量
来源：http://ppm.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://nfy.cashguo.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rqs.fehbvm.com

JS:   process.env.HOME
来源：http://uyi.52xcode.cn

TS:   process.env.HOME
来源：http://tvz.yuxming.cn

Java: System.getenv("HOME")
来源：http://zaw.hammf.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ygm.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://wap.yueranfly.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://moe.zhengqikj.top

[M03] 执行外部命令
来源：http://eov.52xcode.cn


<!-- 参考信息 -->