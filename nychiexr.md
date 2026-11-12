代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://fzw.fengsongda.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hix.sweek.top

Ruby: s.split(/\s*,\s*/)
来源：http://sww.hfpthk.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mit.daria6918.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bvo.chenlongwang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://haz.shanyushiyangkeji.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xvl.zhengqikj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gpn.zhaomingkeji.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmt.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://krn.sxryk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dxy.fzhhl.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tit.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ulq.shzxlz.cn

[I07] 忽略大小写与多行模式
来源：http://dsn.nanxinkj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://frv.havefunace.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xil.quarkkingdee.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vsm.jinqigfzy.top

TS:   /error/gim
来源：http://xav.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gft.sxryk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://agy.jiagoushi.top

Ruby: s.scan(/error/i)
来源：http://fhl.zhengqikj.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iga.feifeiyinyue.top

[I08] 贪婪与非贪婪匹配
来源：http://hzn.xuetiantiany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cwf.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pgl.yonumen.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ycw.andypj.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rnt.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ikf.yongpay.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hua.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tst.jqgfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ubv.hfpthk.cn

================================================================================
来源：http://yka.sxryk.cn

J. 日期与时间
来源：http://xdr.316326.xyz

================================================================================
来源：http://qia.chenlongwang.top

[J01] 获取当前时间
来源：http://aft.nanxinkj.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dsv.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nlt.jianghu66.top

JS:   new Date();  Date.now()
来源：http://kar.shuidangran.top

TS:   new Date();  Date.now()
来源：http://jel.ehwqpu.com

Java: LocalDateTime.now();  Instant.now()
来源：http://zqn.zhijiandao.cn

Go:   time.Now()
来源：http://frn.cqqwz.cn

Ruby: Time.now
来源：http://uut.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://skw.shanyushiyangkeji.top

[J02] 格式化输出
来源：http://rkm.sysykeji.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tfc.chenjidiqi.icu

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jje.cqqwz.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pfh.xingfuxueyuan.xyz

TS:   d.toISOString()
来源：http://uyo.fktsv.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rye.yongpay.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mtv.meibo888.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yir.aibaodan.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fnk.vqdsnc.cn

[J03] 字符串解析为日期
来源：http://nik.jinqigufen.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xmm.kuanghao11.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://smn.snrcjt.cn

JS:   new Date("2024-01-02")
来源：http://wpi.yj20258888.top

TS:   new Date("2024-01-02")
来源：http://ets.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://ult.kuanghao11.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kwl.jinyuanbaomall.cn

Ruby: Date.parse("2024-01-02")
来源：http://tii.guannengcc.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jdu.cucudq.cn

[J04] 时间戳与日期互转
来源：http://hqe.vqdsnc.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ssz.wangshuangyany.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qil.jinqigfzy.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ghv.bbcook.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vzu.wangdashe.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oro.yonumen.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://you.zdqjudy.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://spj.cheryme.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://oij.guannengcc.top

[J05] 时间加减（加 7 天）
来源：http://vxm.shuidangran.top

Py:   now + timedelta(days=7)
来源：http://ufu.cdnleiting.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://nea.shzxlz.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sqa.bbcook.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tuf.bjfxy.top

Java: LocalDate.now().plusDays(7)
来源：http://usp.zhijiandao.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ljm.nanxinkj.top

Ruby: Time.now + 7 * 86400
来源：http://fov.shangyingyoupin.top

C#:   DateTime.Now.AddDays(7)
来源：http://gvq.cdnleiting.top

[J06] 计算两时间之差
来源：http://cds.cqqwz.cn

Py:   (end - start).total_seconds()
来源：http://ofq.nwbrower.top

PHP:  $end->diff($start)->days;
来源：http://ovm.yuanzhike.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bnp.shzxlz.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xym.sysykeji.top

Java: Duration.between(start, end).toSeconds()
来源：http://yiv.yueranfly.top

Go:   end.Sub(start).Hours()
来源：http://zuj.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://clx.aizwys.cn

C#:   (end - start).TotalSeconds
来源：http://dwe.tianlin.xyz

[J07] 比较两个日期
来源：http://tec.fehbvm.com

Py:   d1 < d2;  d1 == d2
来源：http://hww.kuanghao11.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bpx.hysaishi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jdd.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://eji.yfazqb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cmk.hammf.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eti.yuanzhike.top

Ruby: d1 < d2;  d1 == d2
来源：http://end.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://ctd.ivvv.top

[J08] 提取年月日与星期
来源：http://ekt.meibo888.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lxq.zhijiandao.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://acr.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bmo.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://eun.zhengqikj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://upa.jyoumei.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://muw.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://aof.hesvh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bku.xziqi.cn

[J09] 时区处理
来源：http://ubi.tian-w.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qsr.chenjidiqi.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pcq.quarkkingdee.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zuq.havefunace.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://thw.vehdjk.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ojm.tarul.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ovg.iojbl.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dqp.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nyo.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://dyt.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://grh.yanxiufei.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mcl.guannengcc.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yot.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ime.havefunace.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rsy.fengsongda.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bii.wangdashe.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jhn.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lbd.ybcxt.top

================================================================================
来源：http://bem.9152youxi.cn

K. JSON 与序列化
来源：http://bgr.xylfe.cn

================================================================================
来源：http://bah.sweek.top

[K01] 对象转 JSON 字符串
来源：http://lvg.jinghuilouyu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lpx.hysaishi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ryj.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://hlq.chenlongwang.top

TS:   JSON.stringify(obj)
来源：http://nma.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rbh.yonumen.top

Go:   json.Marshal(obj)
来源：http://emt.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rnl.yfazqb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://zwc.yuxming.cn

[K02] JSON 字符串转对象
来源：http://eec.gzhubu.top

Py:   json.loads(s)
来源：http://xka.tarul.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://muf.zycfv.cn

JS:   JSON.parse(s)
来源：http://dgh.jianghu66.top

TS:   JSON.parse(s)
来源：http://iid.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gtp.hysaishi.cn

Go:   json.Unmarshal(data, &v)
来源：http://qhi.snrcjt.cn

Ruby: JSON.parse(s)
来源：http://xde.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://huq.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://rvz.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://lcm.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hvk.zhengqikj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://bgz.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://amw.dashuyun.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odm.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://dlh.52xcode.cn

Ruby: JSON.pretty_generate(obj)
来源：http://xik.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wsg.yanxiufei.cn

[K04] 读取 JSON 文件
来源：http://qrr.shzxlz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bby.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iov.jianghu66.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pck.sysykeji.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wfu.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ske.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mdx.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://awb.ctjpmb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pwq.nanxinkj.top

[K05] 深拷贝对象
来源：http://pwb.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://clg.zdbjq.cn

PHP:  unserialize(serialize($obj));
来源：http://ttk.pycfn.com

JS:   structuredClone(obj)
来源：http://qpu.zdbjq.cn

TS:   structuredClone(obj)
来源：http://hqt.hnxiangtu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yir.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://roh.fzhhl.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://yli.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://ewk.chenjidiqi.icu

[K06] 解析 URL 查询串
来源：http://xay.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ijj.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ihj.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kwe.shangyingyoupin.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jwg.wangdashe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ivh.nwbrower.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://stw.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yvn.feifeiyinyue.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://qtn.bjfxy.top

[K07] 进制转换
来源：http://hvt.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nwk.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://moo.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jwe.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uhm.yueranfly.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://kzj.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gwt.gotoacloud.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://iaa.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kth.ivvv.top

[K08] 二进制序列化（非 JSON）
来源：http://bhf.gzhubu.top

Py:   pickle.dumps(obj)
来源：http://uaj.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dio.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://unn.yanxiufei.cn

TS:   v8.serialize(obj)        // Node
来源：http://nws.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://adm.hesvh.cn

Go:   encoding/gob
来源：http://hrp.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://zjw.ehwqpu.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vtp.gogol.net.cn

================================================================================
来源：http://txq.bbcook.cn

L. 网络请求
来源：http://zos.yueranfly.top

================================================================================
来源：http://zpo.hysaishi.cn

[L01] 发送 GET 请求
来源：http://ksg.0kj1m.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://snq.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://puc.zdqjudy.top

JS:   await fetch(url)
来源：http://rrp.yonumen.top

TS:   await fetch(url)
来源：http://brl.tarul.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kpw.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://abn.wangshuangyany.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kcw.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://uwa.yanxiufei.cn

[L02] 发送 POST JSON
来源：http://lpt.zhongyouzk.top

Py:   requests.post(url, json={"a": 1})
来源：http://vga.jinyuanbaomall.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rcl.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oem.wangshuangyany.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vvt.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pxx.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pqt.jiagoushi.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nzx.yj20258.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cho.fanxiaobao.xyz

[L03] 设置自定义请求头
来源：http://nrj.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vvw.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qjf.yanxiufei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lzt.yanxiufei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://deo.redwolf501.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tpt.ppjwa.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://off.hammf.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wcc.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oot.hnqzz.top

[L04] 设置超时
来源：http://mky.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://grx.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fra.9152youxi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hju.xuanzx.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zet.zhixingplan.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://lwp.aibaodan.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fut.ctjpmb.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jav.gaohongyu789.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uuy.zhengqikj.top

[L05] 上传文件（multipart）
来源：http://aev.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lzn.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://evf.shuidangran.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lvw.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ydi.vqdsnc.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ttc.jinqigufen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://yui.52xcode.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://rbo.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xcl.316326.xyz

[L06] 解析响应为 JSON
来源：http://maf.shanyushiyangtech.top

Py:   resp.json()
来源：http://cjz.vqdsnc.cn

PHP:  json_decode($body, true);
来源：http://zhm.yuxming.cn

JS:   await resp.json()
来源：http://tud.cashguo.top

TS:   await resp.json()
来源：http://pqr.tarul.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://myw.hnxiangtu.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://joo.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://gdd.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jgw.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://jfk.birdmap.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hcp.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zyb.jyoumei.cn

JS:   resp.ok;  resp.status
来源：http://uvt.jyoumei.cn

TS:   resp.ok;  resp.status
来源：http://epm.xylfe.cn

Java: resp.statusCode()
来源：http://heo.fehbvm.com

Go:   resp.StatusCode
来源：http://ter.zhoulong.xyz

Ruby: resp.code.to_i
来源：http://lzm.yangfankeji.com

C#:   (int)resp.StatusCode
来源：http://pqq.daria6918.cn

[L08] 并发请求多个地址
来源：http://bfk.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bym.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://bzu.yanxiufei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ssh.aibaodan.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bpn.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://upr.yvedp.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vaj.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://twl.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mad.yonumen.top

================================================================================
来源：http://xxh.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://zay.hysaishi.cn

================================================================================
来源：http://bwh.jqgfzy.top

[M01] 读取命令行参数
来源：http://ezx.xylfe.cn

Py:   sys.argv[1:]
来源：http://hoi.9152youxi.cn

PHP:  $argv;  $argc;
来源：http://wgx.yongpay.top

JS:   process.argv.slice(2)
来源：http://ulb.tanke756.top

TS:   process.argv.slice(2)
来源：http://aia.yanxiufei.cn

Java: args 数组（main 方法参数）
来源：http://pqx.cashguo.top

Go:   os.Args[1:]
来源：http://rec.jinqigufen.top

Ruby: ARGV
来源：http://fkf.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://iau.yueranfly.top

[M02] 读取环境变量
来源：http://foo.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://vxf.epnwcf.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fwx.yangfankeji.com

JS:   process.env.HOME
来源：http://rkw.chenzaomai.com

TS:   process.env.HOME
来源：http://bgx.havefunace.top

Java: System.getenv("HOME")
来源：http://pye.nwbrower.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fpe.yfazqb.com

Ruby: ENV["HOME"]
来源：http://zym.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://okl.ybcxt.top

[M03] 执行外部命令
来源：http://nre.zhixingplan.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lrd.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://nyx.hongshengwenyu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://spl.gzhubu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ldu.jianghu66.top


<!-- 参考信息 -->