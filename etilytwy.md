代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bai.cheryme.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fsd.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rtw.chenjidiqi.icu

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gyj.jinqigfzy.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dgw.shanyushiyangkeji.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rzi.bjfxy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qow.wangshuangyany.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gfg.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://chq.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://xqu.shanyushiyangtech.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cne.meibo888.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fpv.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qcs.jinqigfzy.top

TS:   /error/gim
来源：http://cqa.cashguo.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://guz.zdqjudy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wtk.wangshuangyany.cn

Ruby: s.scan(/error/i)
来源：http://xuq.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rxi.gotoacloud.top

[I08] 贪婪与非贪婪匹配
来源：http://xba.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://des.shanyushiyangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tvu.gogol.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://igf.aibaodan.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tgz.chenzaomai.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://gbm.jinghuilouyu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sgc.hnxiangtu.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zmb.cqqwz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qkr.zhaomingkeji.xyz

================================================================================
来源：http://cgh.jiagoushi.top

J. 日期与时间
来源：http://hqk.yonumen.top

================================================================================
来源：http://opg.zhixingplan.top

[J01] 获取当前时间
来源：http://dcb.jiagoushi.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://scp.xuetiantiany.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aum.chenlongwang.top

JS:   new Date();  Date.now()
来源：http://caa.316326.xyz

TS:   new Date();  Date.now()
来源：http://arg.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hic.vehdjk.com

Go:   time.Now()
来源：http://erb.aizwys.cn

Ruby: Time.now
来源：http://erm.andypj.xyz

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qbk.daxiang520.top

[J02] 格式化输出
来源：http://unr.bjfxy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wwv.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jaq.wangshuangyany.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rvq.mhx1999.top

TS:   d.toISOString()
来源：http://ifx.mhx1999.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nkl.nanxuanxn.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vqq.hesvh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tax.dianchejie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vxe.pengpengdd.cyou

[J03] 字符串解析为日期
来源：http://nbg.52xcode.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pth.yangfankeji.com

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zev.hfpthk.cn

JS:   new Date("2024-01-02")
来源：http://yjm.yfazqb.com

TS:   new Date("2024-01-02")
来源：http://ygk.xuanzx.com

Java: LocalDate.parse("2024-01-02")
来源：http://sku.nanxinkj.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lpx.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://sny.fktsv.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kmr.yuanzhike.top

[J04] 时间戳与日期互转
来源：http://nre.cashguo.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iuy.chenjidiqi.icu

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ypb.havefunace.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wfy.hnxiangtu.top

TS:   Math.floor(Date.now() / 1000)
来源：http://bek.jinghuilouyu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://huo.tianlin.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nbk.hywenlv.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://srp.xuanzx.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sxq.yongpay.top

[J05] 时间加减（加 7 天）
来源：http://mhf.bbcook.cn

Py:   now + timedelta(days=7)
来源：http://mzu.jqgufenzy.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nay.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wpn.feifeiyinyue.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kqu.mhx1999.top

Java: LocalDate.now().plusDays(7)
来源：http://ign.bjfxy.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vjp.snrcjt.cn

Ruby: Time.now + 7 * 86400
来源：http://xhh.tarul.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wdl.nanxuanxn.top

[J06] 计算两时间之差
来源：http://miv.c1oappe.top

Py:   (end - start).total_seconds()
来源：http://tmx.zhiwuduotai.top

PHP:  $end->diff($start)->days;
来源：http://kut.cheryme.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xih.jqgufenzy.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xqw.ctjpmb.com

Java: Duration.between(start, end).toSeconds()
来源：http://mso.wangshuangyany.cn

Go:   end.Sub(start).Hours()
来源：http://bes.yanxiufei.cn

Ruby: end - start                 # 返回秒数
来源：http://yyg.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://qih.hywenlv.cn

[J07] 比较两个日期
来源：http://fuf.guannengcc.top

Py:   d1 < d2;  d1 == d2
来源：http://npa.meibo888.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://swm.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://tky.tarul.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jnn.zdqjudy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bnf.snrcjt.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://suf.ivvv.top

Ruby: d1 < d2;  d1 == d2
来源：http://vau.mhx1999.top

C#:   d1 < d2;  d1 == d2
来源：http://jig.cucudq.cn

[J08] 提取年月日与星期
来源：http://aer.snrcjt.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dqv.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vom.tanke756.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nuj.hnqzz.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wae.xingfuxueyuan.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://arv.tanke756.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sgy.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ldj.ctjpmb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rqx.tian-w.cn

[J09] 时区处理
来源：http://nbl.haohaochexian.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ikn.jyoumei.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ocl.guowangkeji.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://amk.gaohongyu789.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rxk.52xcode.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vkf.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cio.jlsjyb.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://guy.cqqwz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mvm.guannengcc.top

[J10] 取今天 / 本月第一天
来源：http://hlm.vqdsnc.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ogt.zycfv.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pdf.ppjwa.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://swf.daria6918.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xtn.ydzc1.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kgg.cdnleiting.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qkp.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vtf.guowangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xfg.xylfe.cn

================================================================================
来源：http://ust.uphjek.com

K. JSON 与序列化
来源：http://dwg.shanyushiyangkeji.top

================================================================================
来源：http://zns.c1oappe.top

[K01] 对象转 JSON 字符串
来源：http://swf.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://exh.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dpa.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://gtv.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://urv.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gjo.hfpthk.cn

Go:   json.Marshal(obj)
来源：http://kub.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://vya.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://shc.xinyue.icu

[K02] JSON 字符串转对象
来源：http://gif.jqgufenzy.top

Py:   json.loads(s)
来源：http://hsf.xziqi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pxf.jqgfzy.top

JS:   JSON.parse(s)
来源：http://ndc.c1oappe.top

TS:   JSON.parse(s)
来源：http://uxp.jlsjyb.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iuc.jiagoushi.top

Go:   json.Unmarshal(data, &v)
来源：http://egp.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://jgf.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://smv.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://fyq.aibaodan.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xgp.smart0.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mwv.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dog.svipenyu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hpl.9152youxi.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ylv.zdqjudy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ukg.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://gus.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kpj.shzxlz.cn

[K04] 读取 JSON 文件
来源：http://jts.zhixingplan.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://sxh.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ysi.jinqigufen.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://odi.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mnk.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gmr.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://evq.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cvd.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jsd.fktsv.cn

[K05] 深拷贝对象
来源：http://rff.cqqwz.cn

Py:   copy.deepcopy(obj)
来源：http://fgg.nwbrower.top

PHP:  unserialize(serialize($obj));
来源：http://dho.9152youxi.cn

JS:   structuredClone(obj)
来源：http://zjo.snrcjt.cn

TS:   structuredClone(obj)
来源：http://ymj.shanyushiyangkeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://drd.xziqi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jud.bbcook.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://suz.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://yyr.pycfn.com

[K06] 解析 URL 查询串
来源：http://oay.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zzj.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jdg.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iax.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gmc.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://iob.guowangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vew.hcnkem.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ngx.jqgufenzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gbb.zhijiandao.cn

[K07] 进制转换
来源：http://chk.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dln.zhixingplan.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://irj.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sgp.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://zap.smart0.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zgx.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dpb.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://jan.gzhubu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://frj.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://mfc.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://ruk.yvedp.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://oxg.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://din.feifeiyinyue.top

TS:   v8.serialize(obj)        // Node
来源：http://obx.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yxq.gaohongyu789.top

Go:   encoding/gob
来源：http://dws.pycfn.com

Ruby: Marshal.dump(obj)
来源：http://cde.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wpn.fengsongda.top

================================================================================
来源：http://epb.fanxiaobao.xyz

L. 网络请求
来源：http://cpe.yueranfly.top

================================================================================
来源：http://rnu.9152youxi.cn

[L01] 发送 GET 请求
来源：http://qqo.haohaochexian.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ctq.gaohongyu789.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ywh.zhengqikj.top

JS:   await fetch(url)
来源：http://kvn.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://rnn.bbcook.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jvq.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://gjy.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ttr.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://akz.ppjwa.cn

[L02] 发送 POST JSON
来源：http://zsf.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://jqa.52xcode.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ynr.0kj1m.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ysc.guannengcc.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dqz.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iwh.xziqi.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mvy.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://yzy.shangyingyoupin.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nyp.meibo888.top

[L03] 设置自定义请求头
来源：http://qhw.zycfv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lyq.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tbb.yueranfly.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qet.sufxvd.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ymd.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wli.xylfe.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nny.redwolf501.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wus.meibo888.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://umt.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://rjg.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://uyd.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fqs.zhongyouzk.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vti.wangshuangyany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qtb.chenzaomai.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kej.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fir.ppjwa.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lhf.guannengcc.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jfh.cdnleiting.top

[L05] 上传文件（multipart）
来源：http://jgo.ydzc1.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kxk.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tox.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gbx.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sxf.pengpengdd.cyou

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://sud.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://otq.yuanzhike.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pdu.hnxiangtu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gjc.shzxlz.cn

[L06] 解析响应为 JSON
来源：http://uts.haohaochexian.top

Py:   resp.json()
来源：http://smb.hongshengwenyu.top

PHP:  json_decode($body, true);
来源：http://ryj.gogol.net.cn

JS:   await resp.json()
来源：http://lte.daria6918.cn

TS:   await resp.json()
来源：http://wnd.xylfe.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://eub.nanxuanxn.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://shs.9152youxi.cn

Ruby: JSON.parse(resp.body)
来源：http://lzm.zdqjudy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xnm.jqgfzy.top

[L07] 处理 HTTP 状态码
来源：http://moe.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://djy.birdmap.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ofu.xuanzx.com

JS:   resp.ok;  resp.status
来源：http://kny.ydjk.org.cn

TS:   resp.ok;  resp.status
来源：http://jtu.yvedp.cn

Java: resp.statusCode()
来源：http://ppv.yangfankeji.com

Go:   resp.StatusCode
来源：http://ljh.sysykeji.top

Ruby: resp.code.to_i
来源：http://qpo.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://pmb.ppjwa.cn

[L08] 并发请求多个地址
来源：http://pkt.feifeiyinyue.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://een.ppjwa.cn

PHP:  curl_multi_init() 系列
来源：http://cyt.hywenlv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nwj.yuxming.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ikm.zhiwuduotai.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gcq.zdqjudy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gal.jyoumei.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qfb.jinqigufen.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ote.tian-w.cn

================================================================================
来源：http://ccy.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://dsd.zhengqikj.top

================================================================================
来源：http://dwt.yj20258888.top

[M01] 读取命令行参数
来源：http://qcd.cqqwz.cn

Py:   sys.argv[1:]
来源：http://uup.redwolf501.top

PHP:  $argv;  $argc;
来源：http://ekh.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://ogz.chenlongwang.top

TS:   process.argv.slice(2)
来源：http://krh.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://ixx.ivvv.top

Go:   os.Args[1:]
来源：http://uep.hnxiangtu.top

Ruby: ARGV
来源：http://rjz.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://ktl.sxryk.cn

[M02] 读取环境变量
来源：http://qsk.cheryme.top

Py:   os.environ.get("HOME")
来源：http://aas.wangdashe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zck.mhx1999.top

JS:   process.env.HOME
来源：http://ahm.cqqwz.cn

TS:   process.env.HOME
来源：http://kov.daria6918.cn

Java: System.getenv("HOME")
来源：http://esm.jlsjyb.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uvu.dianchejie.cn

Ruby: ENV["HOME"]
来源：http://bxx.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ruq.yuanzhike.top

[M03] 执行外部命令
来源：http://xug.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yco.fehbvm.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cio.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ijg.gogol.net.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ltq.jqgfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sco.cdnleiting.top

Go:   exec.Command("ls", "-l").Output()
来源：http://tum.smart0.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://rsa.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://rex.pycfn.com


<!-- 参考信息 -->