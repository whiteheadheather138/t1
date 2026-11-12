代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://gel.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zor.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://afs.shzxlz.cn

TS:   s.split(/\s*,\s*/)
来源：http://uun.redwolf501.top

Java: s.split("\\s*,\\s*")
来源：http://khr.daria6918.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ynb.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ode.jinghuilouyu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ydh.zhongyouzk.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kol.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bfu.ivvv.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ylz.zhiwuduotai.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://clw.jyoumei.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xzz.hnqzz.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zyt.yfazqb.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tya.xuanzx.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xvy.yongpay.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://giw.yfazqb.com

[I07] 忽略大小写与多行模式
来源：http://rdt.chenjidiqi.icu

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wsp.fengsongda.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ony.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yao.hongshengwenyu.top

TS:   /error/gim
来源：http://qbu.jqgufenzy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rdo.zhijiandao.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lff.yuxming.cn

Ruby: s.scan(/error/i)
来源：http://ceb.hywenlv.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ktu.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://nbj.c1oappe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://srv.uphjek.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zdh.zhaomingkeji.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ngp.ywan-chungtsiang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rno.xziqi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wei.xylfe.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nim.ppjwa.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bvh.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mjm.gogol.net.cn

================================================================================
来源：http://yez.gaohongyu789.top

J. 日期与时间
来源：http://qnb.epnwcf.com

================================================================================
来源：http://jkj.shanyushiyangtech.top

[J01] 获取当前时间
来源：http://ffj.tarul.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rpp.ydzc1.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dvg.shanyushiyangtech.top

JS:   new Date();  Date.now()
来源：http://zur.hesvh.cn

TS:   new Date();  Date.now()
来源：http://sql.uphjek.com

Java: LocalDateTime.now();  Instant.now()
来源：http://tql.jqgufenzy.top

Go:   time.Now()
来源：http://hdh.hcnkem.com

Ruby: Time.now
来源：http://zse.fzhhl.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tzs.mhx1999.top

[J02] 格式化输出
来源：http://mul.jqgfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hqi.316326.xyz

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cvd.jinghuilouyu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bgo.quarkkingdee.top

TS:   d.toISOString()
来源：http://hkr.daria6918.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://egs.yvedp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fsd.mhx1999.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hif.jqgfzy.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wvo.wangdashe.top

[J03] 字符串解析为日期
来源：http://buv.chenlongwang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gta.316326.xyz

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yql.0kj1m.cn

JS:   new Date("2024-01-02")
来源：http://yki.xylfe.cn

TS:   new Date("2024-01-02")
来源：http://cdd.jqgfzy.top

Java: LocalDate.parse("2024-01-02")
来源：http://zrh.tian-w.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://rnj.xingfuxueyuan.xyz

Ruby: Date.parse("2024-01-02")
来源：http://lkm.kuanghao11.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fzu.ctjpmb.com

[J04] 时间戳与日期互转
来源：http://evg.zhixingplan.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zsn.ctjpmb.com

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zub.nanxinkj.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eql.cheryme.top

TS:   Math.floor(Date.now() / 1000)
来源：http://son.snrcjt.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hrx.hongshengwenyu.top

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://dva.316326.xyz

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zbq.pycfn.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://usc.yj20258888.top

[J05] 时间加减（加 7 天）
来源：http://snk.pengpengdd.cyou

Py:   now + timedelta(days=7)
来源：http://lxq.ybcxt.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://sxh.sufxvd.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eyz.yanxiufei.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://keq.yj20258.top

Java: LocalDate.now().plusDays(7)
来源：http://nsm.smart0.xyz

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vtl.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://uib.shanyushiyangtech.top

C#:   DateTime.Now.AddDays(7)
来源：http://mdr.fzhhl.top

[J06] 计算两时间之差
来源：http://zep.jiagoushi.top

Py:   (end - start).total_seconds()
来源：http://msa.epnwcf.com

PHP:  $end->diff($start)->days;
来源：http://nqp.yuxming.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gxu.sufxvd.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qgl.shangyingyoupin.top

Java: Duration.between(start, end).toSeconds()
来源：http://jrb.guannengcc.top

Go:   end.Sub(start).Hours()
来源：http://bac.ydzc1.top

Ruby: end - start                 # 返回秒数
来源：http://syo.mhx1999.top

C#:   (end - start).TotalSeconds
来源：http://non.xuanzx.com

[J07] 比较两个日期
来源：http://mdw.dashuyun.cn

Py:   d1 < d2;  d1 == d2
来源：http://efb.jqgufenzy.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://xdx.zdqjudy.top

JS:   d1.getTime() < d2.getTime()
来源：http://obl.gogol.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://djk.jianghu66.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qga.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wxo.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://dhm.zhongyouzk.top

C#:   d1 < d2;  d1 == d2
来源：http://ugg.yueranfly.top

[J08] 提取年月日与星期
来源：http://bgu.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gnd.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eud.52xcode.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cvt.jlsjyb.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yhl.ywan-chungtsiang.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dns.ivvv.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dmu.shanyushiyangkeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uot.ivvv.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qsa.fktsv.cn

[J09] 时区处理
来源：http://acw.hongshengwenyu.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qwn.cheryme.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ndo.aibaodan.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://psc.sysykeji.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzy.smart0.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gox.vqdsnc.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rfs.fzhhl.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ufs.hywenlv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xxs.feifeiyinyue.top

[J10] 取今天 / 本月第一天
来源：http://hqi.yueranfly.top

Py:   date.today();  date.today().replace(day=1)
来源：http://vfc.hfpthk.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qdf.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kyt.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cad.gotoacloud.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ell.gaohongyu789.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jcg.jianghu66.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gpo.hnxiangtu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ext.pycfn.com

================================================================================
来源：http://vlc.yueranfly.top

K. JSON 与序列化
来源：http://xrm.uphjek.com

================================================================================
来源：http://tom.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://xmv.316326.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fov.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://chy.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://tay.guowangkeji.top

TS:   JSON.stringify(obj)
来源：http://zcl.yangfankeji.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://opr.daria6918.cn

Go:   json.Marshal(obj)
来源：http://hby.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://drd.zhengqikj.top

C#:   JsonSerializer.Serialize(obj)
来源：http://gvp.birdmap.top

[K02] JSON 字符串转对象
来源：http://bws.yuxming.cn

Py:   json.loads(s)
来源：http://jvc.xuetiantiany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pat.daria6918.cn

JS:   JSON.parse(s)
来源：http://gpq.guannengcc.top

TS:   JSON.parse(s)
来源：http://tad.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://aqd.zhengqikj.top

Go:   json.Unmarshal(data, &v)
来源：http://yjm.xingfuxueyuan.xyz

Ruby: JSON.parse(s)
来源：http://uta.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oxm.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://mok.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yhf.zhijiandao.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ayj.havefunace.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cty.yonumen.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ceb.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rqs.jqgufenzy.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://uex.zhijiandao.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cen.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pry.nwbrower.top

[K04] 读取 JSON 文件
来源：http://wot.nwbrower.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://nbr.zhoulong.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cmp.daxiang520.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kke.xuanzx.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nom.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ggo.vqdsnc.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tko.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cck.nanxuanxn.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fzz.meibo888.top

[K05] 深拷贝对象
来源：http://zch.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://fde.yueranfly.top

PHP:  unserialize(serialize($obj));
来源：http://eah.316326.xyz

JS:   structuredClone(obj)
来源：http://bnz.fehbvm.com

TS:   structuredClone(obj)
来源：http://ymp.uphjek.com

Java: // 手写拷贝构造，或序列化往返
来源：http://odq.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ipu.ywan-chungtsiang.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://qrt.mhx1999.top

C#:   // 序列化往返，或自定义 Clone
来源：http://blf.ppjwa.cn

[K06] 解析 URL 查询串
来源：http://ord.52xcode.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rli.nanxinkj.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lbs.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ncu.ybcxt.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://iub.tian-w.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uai.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jkc.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://euf.jinqigfzy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bel.zhiwuduotai.top

[K07] 进制转换
来源：http://gtm.haohaochexian.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://rnb.cucudq.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dsi.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cvm.tarul.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nrt.ybcxt.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tyz.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://akn.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://myq.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://idg.wangdashe.top

[K08] 二进制序列化（非 JSON）
来源：http://yzw.cheryme.top

Py:   pickle.dumps(obj)
来源：http://lie.jqgufenzy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://rlw.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://pqt.shuidangran.top

TS:   v8.serialize(obj)        // Node
来源：http://npv.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://byp.daria6918.cn

Go:   encoding/gob
来源：http://fdq.guowangkeji.top

Ruby: Marshal.dump(obj)
来源：http://kyt.yj20258888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wlb.vqdsnc.cn

================================================================================
来源：http://fcf.cqqwz.cn

L. 网络请求
来源：http://xpn.aibaodan.cn

================================================================================
来源：http://sqa.sufxvd.cn

[L01] 发送 GET 请求
来源：http://wxo.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pyx.zhaomingkeji.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mvq.jinghuilouyu.cn

JS:   await fetch(url)
来源：http://keo.sysykeji.top

TS:   await fetch(url)
来源：http://sae.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qvs.bbcook.cn

Go:   resp, err := http.Get(url)
来源：http://ypy.hammf.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://npu.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pku.hongshengwenyu.top

[L02] 发送 POST JSON
来源：http://ecs.jiagoushi.top

Py:   requests.post(url, json={"a": 1})
来源：http://nhi.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hml.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://reg.pycfn.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zap.0kj1m.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xwh.tarul.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://quh.yj202588.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aip.c1oappe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uvj.yueranfly.top

[L03] 设置自定义请求头
来源：http://qeg.vehdjk.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qiu.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ugs.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nnv.zycfv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pgg.gaohongyu789.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ysl.gzhubu.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ylx.zhiwuduotai.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nid.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rko.yj20258.top

[L04] 设置超时
来源：http://riu.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://sow.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ipy.ydjk.org.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tff.yangfankeji.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mel.fengsongda.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://suq.pengpengdd.cyou

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qge.hnxiangtu.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sec.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ixu.cucudq.cn

[L05] 上传文件（multipart）
来源：http://lqn.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qtv.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://khj.yanxiufei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gtq.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ctk.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pjv.zhixingplan.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fhd.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vhk.fanxiaobao.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://phm.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://urz.iojbl.cn

Py:   resp.json()
来源：http://ems.aibaodan.cn

PHP:  json_decode($body, true);
来源：http://qtz.meibo888.top

JS:   await resp.json()
来源：http://zxz.yvedp.cn

TS:   await resp.json()
来源：http://kkg.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://aua.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://oik.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://bva.guowangkeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jaf.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://qur.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wfp.tianlin.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gar.yvedp.cn

JS:   resp.ok;  resp.status
来源：http://nug.hywenlv.cn

TS:   resp.ok;  resp.status
来源：http://wol.hnxiangtu.top

Java: resp.statusCode()
来源：http://fxl.zdbjq.cn

Go:   resp.StatusCode
来源：http://tpp.svipenyu.cn

Ruby: resp.code.to_i
来源：http://ene.vehdjk.com

C#:   (int)resp.StatusCode
来源：http://btd.aizwys.cn

[L08] 并发请求多个地址
来源：http://tml.hammf.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lnb.zdqjudy.top

PHP:  curl_multi_init() 系列
来源：http://lnv.zycfv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://roi.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nmj.jqgufenzy.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://iry.vqdsnc.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oog.guannengcc.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gen.tianlin.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cit.yj20258888.top

================================================================================
来源：http://sxp.tanke756.top

M. 命令行 / 进程 / 环境
来源：http://stc.yongpay.top

================================================================================
来源：http://zhj.fanxiaobao.xyz

[M01] 读取命令行参数
来源：http://gyz.ivvv.top

Py:   sys.argv[1:]
来源：http://ier.xuanzx.com

PHP:  $argv;  $argc;
来源：http://oui.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://wbc.birdmap.top

TS:   process.argv.slice(2)
来源：http://tnc.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://nkf.tian-w.cn

Go:   os.Args[1:]
来源：http://gqm.shanyushiyangkeji.top

Ruby: ARGV
来源：http://sfr.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://wja.snrcjt.cn

[M02] 读取环境变量
来源：http://eum.cashguo.top

Py:   os.environ.get("HOME")
来源：http://vmd.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cqz.xuetiantiany.cn

JS:   process.env.HOME
来源：http://xtn.yj202588.top

TS:   process.env.HOME
来源：http://sin.sweek.top

Java: System.getenv("HOME")
来源：http://piy.pycfn.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://asu.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://pwu.xingfuxueyuan.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gnp.nanxinkj.top

[M03] 执行外部命令
来源：http://xyk.jinqigfzy.top


<!-- 参考信息 -->