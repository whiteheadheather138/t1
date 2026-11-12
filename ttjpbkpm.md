代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vsx.yueranfly.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hpi.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xtr.yueranfly.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jck.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wax.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vea.9152youxi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://abb.daxiang520.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zcg.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vvo.jqgufenzy.top

[I07] 忽略大小写与多行模式
来源：http://icv.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://awi.yfazqb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bid.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nzo.xinyue.icu

TS:   /error/gim
来源：http://kki.shanyushiyangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ium.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kwr.yj20258.top

Ruby: s.scan(/error/i)
来源：http://xpa.mhx1999.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tmd.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://wtl.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gup.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uni.xinyue.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jga.havefunace.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://thv.tian-w.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nwf.gzhubu.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xyy.nanxinkj.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pgu.hammf.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://btn.zdbjq.cn

================================================================================
来源：http://dco.cheryme.top

J. 日期与时间
来源：http://kxw.dianchejie.cn

================================================================================
来源：http://uwd.xuanzx.com

[J01] 获取当前时间
来源：http://tuf.iojbl.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://odn.guowangkeji.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mey.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://yvy.vehdjk.com

TS:   new Date();  Date.now()
来源：http://zal.gaohongyu789.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bqc.sysykeji.top

Go:   time.Now()
来源：http://kyl.zycfv.cn

Ruby: Time.now
来源：http://szs.quarkkingdee.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ajp.vqdsnc.cn

[J02] 格式化输出
来源：http://rbf.shangyingyoupin.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pqd.smart0.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tqo.sysykeji.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hxj.hesvh.cn

TS:   d.toISOString()
来源：http://yey.havefunace.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bjn.vehdjk.com

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://auc.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pfd.sweek.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://jdt.andypj.xyz

[J03] 字符串解析为日期
来源：http://pop.xziqi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nss.hnxiangtu.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://whg.jqgufenzy.top

JS:   new Date("2024-01-02")
来源：http://adt.epnwcf.com

TS:   new Date("2024-01-02")
来源：http://wym.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zzs.chenjidiqi.icu

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zcv.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://gpw.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://emg.zhijiandao.cn

[J04] 时间戳与日期互转
来源：http://dak.0kj1m.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://val.yuanzhike.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qix.cucudq.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vol.hesvh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ztc.hfpthk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nre.jinyuanbaomall.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ipv.chenlongwang.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ywg.meibo888.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wkq.zhiwuduotai.top

[J05] 时间加减（加 7 天）
来源：http://opn.0kj1m.cn

Py:   now + timedelta(days=7)
来源：http://zah.yuanzhike.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://tio.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://bhf.iojbl.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wxs.ehwqpu.com

Java: LocalDate.now().plusDays(7)
来源：http://oft.fanxiaobao.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jzi.hysaishi.cn

Ruby: Time.now + 7 * 86400
来源：http://znj.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://yrl.hongshengwenyu.top

[J06] 计算两时间之差
来源：http://mbz.hesvh.cn

Py:   (end - start).total_seconds()
来源：http://ljs.feifeiyinyue.top

PHP:  $end->diff($start)->days;
来源：http://ryf.mhx1999.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bck.mhx1999.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ism.cqqwz.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gkl.ybcxt.top

Go:   end.Sub(start).Hours()
来源：http://kdu.wangdashe.top

Ruby: end - start                 # 返回秒数
来源：http://olv.jinqigufen.top

C#:   (end - start).TotalSeconds
来源：http://wwn.gaohongyu789.top

[J07] 比较两个日期
来源：http://mry.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://uks.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jfn.haohaochexian.top

JS:   d1.getTime() < d2.getTime()
来源：http://nrb.epnwcf.com

TS:   d1.getTime() < d2.getTime()
来源：http://srj.jiagoushi.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ynw.epnwcf.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hcn.tian-w.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jmm.tian-w.cn

C#:   d1 < d2;  d1 == d2
来源：http://uin.sufxvd.cn

[J08] 提取年月日与星期
来源：http://zcr.wangdashe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ztq.jqgfzy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nvz.ppjwa.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jsp.9152youxi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ayi.hammf.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mvq.epnwcf.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://plb.sweek.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gvi.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bny.9152youxi.cn

[J09] 时区处理
来源：http://oen.sweek.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qcf.fehbvm.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pgv.xylfe.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://avh.zdqjudy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qri.ppjwa.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yfz.wangshuangyany.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pcn.jinqigfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jse.ivvv.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ifu.haohaochexian.top

[J10] 取今天 / 本月第一天
来源：http://mas.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pxt.gaohongyu789.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ybp.ydjk.org.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://akh.yuxming.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://slp.fehbvm.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cxn.sufxvd.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qct.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ppb.birdmap.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://cvh.gzhubu.top

================================================================================
来源：http://jjs.jinqigufen.top

K. JSON 与序列化
来源：http://sgx.hammf.cn

================================================================================
来源：http://bfp.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://shh.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pzy.9152youxi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pbm.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://pik.fengsongda.top

TS:   JSON.stringify(obj)
来源：http://hgx.yfazqb.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://alj.daxiang520.top

Go:   json.Marshal(obj)
来源：http://cll.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://jnt.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://pxx.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://kqt.hywenlv.cn

Py:   json.loads(s)
来源：http://aip.aibaodan.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wup.fktsv.cn

JS:   JSON.parse(s)
来源：http://vtu.chenzaomai.com

TS:   JSON.parse(s)
来源：http://iig.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hdf.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://cnk.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://fml.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://elq.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://czj.nanxinkj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mfx.fanxiaobao.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qiu.vqdsnc.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xlw.zhiwuduotai.top

TS:   JSON.stringify(obj, null, 2)
来源：http://mwp.sweek.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kjr.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xjv.fanxiaobao.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://prd.hesvh.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pyq.hnqzz.top

[K04] 读取 JSON 文件
来源：http://uec.chenzaomai.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://stm.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxo.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssu.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://frt.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xpu.nanxinkj.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hmt.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jxz.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rai.sufxvd.cn

[K05] 深拷贝对象
来源：http://com.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://ber.yanxiufei.cn

PHP:  unserialize(serialize($obj));
来源：http://qij.zdqjudy.top

JS:   structuredClone(obj)
来源：http://fkn.jqgfzy.top

TS:   structuredClone(obj)
来源：http://xyb.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zun.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oyw.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://per.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yqm.sjlbkw.cn

[K06] 解析 URL 查询串
来源：http://khx.yfazqb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zta.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nxv.wangdashe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qjq.ehwqpu.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nke.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fcp.yvedp.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bro.jinqigfzy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ior.zycfv.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://oqv.yonumen.top

[K07] 进制转换
来源：http://bxm.jlsjyb.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmm.tianlin.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yqp.52xcode.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tze.aibaodan.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qkh.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dux.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://sxe.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://syn.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://dgx.pycfn.com

[K08] 二进制序列化（非 JSON）
来源：http://ggq.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://gol.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fnj.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://pox.xingfuxueyuan.xyz

TS:   v8.serialize(obj)        // Node
来源：http://brh.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yop.sweek.top

Go:   encoding/gob
来源：http://syy.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://png.fanxiaobao.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mvm.sysykeji.top

================================================================================
来源：http://xde.vqdsnc.cn

L. 网络请求
来源：http://ynp.smart0.xyz

================================================================================
来源：http://kem.zhixingplan.top

[L01] 发送 GET 请求
来源：http://nkr.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rgg.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yoy.quarkkingdee.top

JS:   await fetch(url)
来源：http://ffj.chenzaomai.com

TS:   await fetch(url)
来源：http://gap.zhiwuduotai.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vms.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://zqr.yangfankeji.com

Ruby: Net::HTTP.get(URI(url))
来源：http://asi.haohaochexian.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rei.ehwqpu.com

[L02] 发送 POST JSON
来源：http://ggl.yj20258888.top

Py:   requests.post(url, json={"a": 1})
来源：http://xmt.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ddv.havefunace.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lgw.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sar.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yta.bbcook.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://uvh.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rep.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fyc.daria6918.cn

[L03] 设置自定义请求头
来源：http://mmp.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kpw.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ydm.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://odn.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://amc.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gdt.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://osl.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rjn.daxiang520.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mbr.52xcode.cn

[L04] 设置超时
来源：http://hlt.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://klh.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cvl.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xdr.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nzr.mhx1999.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tiv.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://omk.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kqk.shanyushiyangkeji.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://upd.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://jiv.meibo888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gpr.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ymy.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aoa.ydzc1.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bfs.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rqb.cqqwz.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vqk.jqgufenzy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://klc.hywenlv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://voz.dashuyun.cn

[L06] 解析响应为 JSON
来源：http://xjo.zhoulong.xyz

Py:   resp.json()
来源：http://vnc.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://jhm.cheryme.top

JS:   await resp.json()
来源：http://quj.hammf.cn

TS:   await resp.json()
来源：http://vqc.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rog.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gca.wangshuangyany.cn

Ruby: JSON.parse(resp.body)
来源：http://rci.dianchejie.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ows.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://boy.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://udz.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bln.yanxiufei.cn

JS:   resp.ok;  resp.status
来源：http://mrw.zhoulong.xyz

TS:   resp.ok;  resp.status
来源：http://xhx.hysaishi.cn

Java: resp.statusCode()
来源：http://lqd.smart0.xyz

Go:   resp.StatusCode
来源：http://zkd.sysykeji.top

Ruby: resp.code.to_i
来源：http://sed.meibo888.top

C#:   (int)resp.StatusCode
来源：http://pyc.jiagoushi.top

[L08] 并发请求多个地址
来源：http://gxb.yj202588.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://udj.hysaishi.cn

PHP:  curl_multi_init() 系列
来源：http://wfr.yuanzhike.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iyx.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tqr.gzhubu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://deb.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iqz.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://isv.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ooa.cqqwz.cn

================================================================================
来源：http://wsm.xylfe.cn

M. 命令行 / 进程 / 环境
来源：http://wvg.ywan-chungtsiang.top

================================================================================
来源：http://cfp.9152youxi.cn

[M01] 读取命令行参数
来源：http://ryo.ydzc1.top

Py:   sys.argv[1:]
来源：http://zwb.ppjwa.cn

PHP:  $argv;  $argc;
来源：http://rpa.yueranfly.top

JS:   process.argv.slice(2)
来源：http://nym.jinghuilouyu.cn

TS:   process.argv.slice(2)
来源：http://ocx.cucudq.cn

Java: args 数组（main 方法参数）
来源：http://qdl.cqqwz.cn

Go:   os.Args[1:]
来源：http://zsb.daxiang520.top

Ruby: ARGV
来源：http://mtz.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://vmg.316326.xyz

[M02] 读取环境变量
来源：http://eui.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://wyc.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nzp.quarkkingdee.top

JS:   process.env.HOME
来源：http://xsh.zhixingplan.top

TS:   process.env.HOME
来源：http://ias.jqgfzy.top

Java: System.getenv("HOME")
来源：http://jie.daxiang520.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ngp.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://puw.tarul.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pqs.jqgufenzy.top

[M03] 执行外部命令
来源：http://bks.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://izi.wangdashe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ssd.zhijiandao.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://qhi.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://kmh.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kfw.kuanghao11.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://aqi.gotoacloud.top

Ruby: system("ls -l");  `ls -l`
来源：http://qbc.zdqjudy.top

C#:   Process.Start("ls", "-l");
来源：http://rhq.ydjk.org.cn


<!-- 参考信息 -->