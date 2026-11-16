代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://clx.aizwys.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oky.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://yae.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sqa.hnxiangtu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bsa.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gbu.hnqzz.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kif.hesvh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mlq.shanyushiyangtech.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ctz.snrcjt.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://atv.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pvo.jinqigfzy.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zuu.bjfxy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://opr.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://mlr.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ulv.xinyue.icu

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zsg.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yes.haohaochexian.top

TS:   /error/gim
来源：http://dny.52xcode.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nrq.hysaishi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wza.ctjpmb.com

Ruby: s.scan(/error/i)
来源：http://pxj.ppjwa.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wlt.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://eme.meibo888.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bzl.zhixingplan.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nne.cqqwz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ofv.hongshengwenyu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wcy.jlsjyb.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lib.jlsjyb.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ryc.havefunace.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ivn.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cxp.epnwcf.com

================================================================================
来源：http://cuu.yanxiufei.cn

J. 日期与时间
来源：http://omx.xylfe.cn

================================================================================
来源：http://nju.c1oappe.top

[J01] 获取当前时间
来源：http://usi.xuanzx.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://qni.xinyue.icu

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://drv.cqqwz.cn

JS:   new Date();  Date.now()
来源：http://zgw.ydjk.org.cn

TS:   new Date();  Date.now()
来源：http://shz.yongpay.top

Java: LocalDateTime.now();  Instant.now()
来源：http://vep.jqgufenzy.top

Go:   time.Now()
来源：http://smr.cdnleiting.top

Ruby: Time.now
来源：http://kyh.guowangkeji.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ilv.ywan-chungtsiang.top

[J02] 格式化输出
来源：http://hiy.hywenlv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vls.hesvh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mha.cdnleiting.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://crx.ctjpmb.com

TS:   d.toISOString()
来源：http://knb.tarul.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dyp.sjlbkw.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pgt.yonumen.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sph.yj202588.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vyv.quarkkingdee.top

[J03] 字符串解析为日期
来源：http://xam.tarul.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://aop.jlsjyb.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wjl.nanxuanxn.top

JS:   new Date("2024-01-02")
来源：http://hgf.hammf.cn

TS:   new Date("2024-01-02")
来源：http://sre.tarul.cn

Java: LocalDate.parse("2024-01-02")
来源：http://www.redwolf501.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hov.fzhhl.top

Ruby: Date.parse("2024-01-02")
来源：http://trk.daxiang520.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xht.ydzc1.top

[J04] 时间戳与日期互转
来源：http://wjd.yfazqb.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pgz.sysykeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mmu.kuanghao11.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dzo.shanyushiyangkeji.top

TS:   Math.floor(Date.now() / 1000)
来源：http://gjf.shanyushiyangkeji.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hvc.xinyue.icu

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jqo.haohaochexian.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qsm.ydzc1.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yyk.gaohongyu789.top

[J05] 时间加减（加 7 天）
来源：http://qxa.quarkkingdee.top

Py:   now + timedelta(days=7)
来源：http://jdw.9152youxi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ebm.cashguo.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://flb.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lex.zhijiandao.cn

Java: LocalDate.now().plusDays(7)
来源：http://vva.redwolf501.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://niu.hnxiangtu.top

Ruby: Time.now + 7 * 86400
来源：http://khp.shuidangran.top

C#:   DateTime.Now.AddDays(7)
来源：http://phy.fzhhl.top

[J06] 计算两时间之差
来源：http://xyo.yonumen.top

Py:   (end - start).total_seconds()
来源：http://zmb.guowangkeji.top

PHP:  $end->diff($start)->days;
来源：http://jrv.cdnleiting.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mol.tanke756.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qtl.chenzaomai.com

Java: Duration.between(start, end).toSeconds()
来源：http://cne.zhengqikj.top

Go:   end.Sub(start).Hours()
来源：http://yxm.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://vst.meibo888.top

C#:   (end - start).TotalSeconds
来源：http://gvd.xylfe.cn

[J07] 比较两个日期
来源：http://azo.ehwqpu.com

Py:   d1 < d2;  d1 == d2
来源：http://ylg.wangdashe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lud.ppjwa.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kip.chenjidiqi.icu

TS:   d1.getTime() < d2.getTime()
来源：http://gwu.hnxiangtu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://btl.cqqwz.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xoo.wangdashe.top

Ruby: d1 < d2;  d1 == d2
来源：http://cij.yvedp.cn

C#:   d1 < d2;  d1 == d2
来源：http://bmj.fengsongda.top

[J08] 提取年月日与星期
来源：http://vqm.jqgfzy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qnn.bjfxy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://uli.shanyushiyangtech.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tfc.hammf.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dcv.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yjd.daxiang520.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jou.yj202588.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dcb.daxiang520.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lzk.iojbl.cn

[J09] 时区处理
来源：http://hls.meibo888.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qfw.dashuyun.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wgk.gzhubu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://azj.jinqigfzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fay.zhixingplan.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zjd.hysaishi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pry.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hzm.shzxlz.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ewx.yj20258.top

[J10] 取今天 / 本月第一天
来源：http://nil.gotoacloud.top

Py:   date.today();  date.today().replace(day=1)
来源：http://pvz.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bce.tian-w.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://egn.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cky.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wtu.fehbvm.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ygk.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bdj.jlsjyb.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://unk.svipenyu.cn

================================================================================
来源：http://toh.bjfxy.top

K. JSON 与序列化
来源：http://qnv.nanxuanxn.top

================================================================================
来源：http://jom.ppjwa.cn

[K01] 对象转 JSON 字符串
来源：http://avm.zhaomingkeji.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yti.ppjwa.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uzd.zdqjudy.top

JS:   JSON.stringify(obj)
来源：http://olo.epnwcf.com

TS:   JSON.stringify(obj)
来源：http://yhi.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cij.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://tqs.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://igf.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vjx.yanxiufei.cn

[K02] JSON 字符串转对象
来源：http://zdf.jyoumei.cn

Py:   json.loads(s)
来源：http://net.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wlv.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://mjo.ywan-chungtsiang.top

TS:   JSON.parse(s)
来源：http://eyn.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://llo.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://cdr.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://okz.0kj1m.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ghn.meibo888.top

[K03] JSON 美化输出（带缩进）
来源：http://hda.wangdashe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xpu.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hpg.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://yba.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://eif.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xdj.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kmk.quarkkingdee.top

Ruby: JSON.pretty_generate(obj)
来源：http://abh.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lxy.pycfn.com

[K04] 读取 JSON 文件
来源：http://vbh.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ckk.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cjy.smart0.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qho.wangdashe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pbz.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://eji.cashguo.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ksx.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ldz.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xjk.nwbrower.top

[K05] 深拷贝对象
来源：http://qkm.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://qhq.sysykeji.top

PHP:  unserialize(serialize($obj));
来源：http://zmf.chenlongwang.top

JS:   structuredClone(obj)
来源：http://cjo.yvedp.cn

TS:   structuredClone(obj)
来源：http://xhb.jianghu66.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ylz.fengsongda.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://duy.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qyk.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://msi.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://xpc.zdbjq.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jej.zhijiandao.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rtw.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ask.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mtk.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xwl.shzxlz.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kri.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://atp.zhengqikj.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wiv.0kj1m.cn

[K07] 进制转换
来源：http://kgg.hfpthk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xtf.epnwcf.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tjy.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tyv.havefunace.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://npd.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zce.yj20258.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://bxz.tarul.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://had.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://krv.tanke756.top

[K08] 二进制序列化（非 JSON）
来源：http://nrt.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://umw.fktsv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ugs.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://kmq.zhongyouzk.top

TS:   v8.serialize(obj)        // Node
来源：http://elo.shzxlz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zrl.hnxiangtu.top

Go:   encoding/gob
来源：http://aeo.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://oot.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://itx.havefunace.top

================================================================================
来源：http://loc.chenzaomai.com

L. 网络请求
来源：http://uhk.jiagoushi.top

================================================================================
来源：http://qpv.daria6918.cn

[L01] 发送 GET 请求
来源：http://zhu.52xcode.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oaa.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tto.aizwys.cn

JS:   await fetch(url)
来源：http://dqi.chenzaomai.com

TS:   await fetch(url)
来源：http://flm.hcnkem.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://cij.yueranfly.top

Go:   resp, err := http.Get(url)
来源：http://kwf.kuanghao11.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dwp.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hhc.aibaodan.cn

[L02] 发送 POST JSON
来源：http://ogq.daxiang520.top

Py:   requests.post(url, json={"a": 1})
来源：http://cqe.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qpm.sufxvd.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cpu.shzxlz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vhm.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://azy.redwolf501.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dzq.yongpay.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://syp.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://stg.gzhubu.top

[L03] 设置自定义请求头
来源：http://lvz.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://svk.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zcg.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dhs.daria6918.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cgp.uphjek.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ntb.tianlin.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wqt.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sbq.fengsongda.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mxr.haohaochexian.top

[L04] 设置超时
来源：http://yms.ywan-chungtsiang.top

Py:   requests.get(url, timeout=5)
来源：http://dhq.yangfankeji.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tzw.sweek.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zxk.cheryme.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zdf.vehdjk.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ldg.redwolf501.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iiv.iojbl.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mgv.wangshuangyany.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vzh.redwolf501.top

[L05] 上传文件（multipart）
来源：http://vrs.hywenlv.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqt.redwolf501.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zuf.ppjwa.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dka.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dye.havefunace.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qrj.ybcxt.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ocv.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nag.epnwcf.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wgr.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://ldx.hcnkem.com

Py:   resp.json()
来源：http://rmh.ctjpmb.com

PHP:  json_decode($body, true);
来源：http://jto.aibaodan.cn

JS:   await resp.json()
来源：http://zgm.yj20258.top

TS:   await resp.json()
来源：http://neo.daxiang520.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://apr.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://iyj.jinqigufen.top

Ruby: JSON.parse(resp.body)
来源：http://jir.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ryn.yvedp.cn

[L07] 处理 HTTP 状态码
来源：http://xyn.cdnleiting.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://psb.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bgd.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://phm.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://sbs.yangfankeji.com

Java: resp.statusCode()
来源：http://afo.xuetiantiany.cn

Go:   resp.StatusCode
来源：http://xqq.andypj.xyz

Ruby: resp.code.to_i
来源：http://nhj.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://bpq.epnwcf.com

[L08] 并发请求多个地址
来源：http://ojv.guannengcc.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ibk.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://dla.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwq.fengsongda.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://huh.xylfe.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://duz.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zxi.52xcode.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mhk.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://suy.hongshengwenyu.top

================================================================================
来源：http://akd.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://ujo.fehbvm.com

================================================================================
来源：http://dst.mhx1999.top

[M01] 读取命令行参数
来源：http://uks.cdnleiting.top

Py:   sys.argv[1:]
来源：http://aqu.jianghu66.top

PHP:  $argv;  $argc;
来源：http://pau.ydzc1.top

JS:   process.argv.slice(2)
来源：http://zgb.xylfe.cn

TS:   process.argv.slice(2)
来源：http://ire.aibaodan.cn

Java: args 数组（main 方法参数）
来源：http://blx.cheryme.top

Go:   os.Args[1:]
来源：http://fci.ydzc1.top

Ruby: ARGV
来源：http://opn.zhaomingkeji.xyz

C#:   args 数组（Main 方法参数）
来源：http://zha.jiagoushi.top

[M02] 读取环境变量
来源：http://qrt.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://xns.316326.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cpy.smart0.xyz

JS:   process.env.HOME
来源：http://way.birdmap.top

TS:   process.env.HOME
来源：http://ddw.fengsongda.top

Java: System.getenv("HOME")
来源：http://nsn.zdqjudy.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yns.gotoacloud.top

Ruby: ENV["HOME"]
来源：http://tij.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://txt.daxiang520.top

[M03] 执行外部命令
来源：http://fan.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ttw.kuanghao11.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dno.gotoacloud.top

JS:   child_process.execSync("ls -l").toString()
来源：http://hix.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://tio.epnwcf.com


<!-- 参考信息 -->