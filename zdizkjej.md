代发 wailian999

Py:   re.split(r"\s*,\s*", s)
来源：http://nhj.xuetiantiany.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rfj.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://hhe.kuanghao11.cn

TS:   s.split(/\s*,\s*/)
来源：http://nkc.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://iti.hammf.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://akg.tian-w.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xru.snrcjt.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ago.bjfxy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://efd.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://neb.fzhhl.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bmx.xuetiantiany.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tic.gogol.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgb.andypj.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fqc.yangfankeji.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://esv.hnxiangtu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cpo.sjlbkw.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bal.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://bxy.chenlongwang.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://muv.cqqwz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xcv.mhx1999.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tnv.hcnkem.com

TS:   /error/gim
来源：http://mfe.xingfuxueyuan.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ayp.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tks.ydjk.org.cn

Ruby: s.scan(/error/i)
来源：http://ukg.xylfe.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xyh.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://tun.shzxlz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wei.hywenlv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://swn.chenjidiqi.icu

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vzo.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kho.zhongyouzk.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wem.guannengcc.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wad.daria6918.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tvc.vehdjk.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ivt.jqgfzy.top

================================================================================
来源：http://fmy.ywan-chungtsiang.top

J. 日期与时间
来源：http://rpx.hnqzz.top

================================================================================
来源：http://mpn.jqgfzy.top

[J01] 获取当前时间
来源：http://cug.uphjek.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://azt.nwbrower.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jpw.sweek.top

JS:   new Date();  Date.now()
来源：http://kqi.hysaishi.cn

TS:   new Date();  Date.now()
来源：http://oqx.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://oor.svipenyu.cn

Go:   time.Now()
来源：http://ujk.redwolf501.top

Ruby: Time.now
来源：http://wud.wangshuangyany.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eal.shangyingyoupin.top

[J02] 格式化输出
来源：http://hoo.zdbjq.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uec.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iok.9152youxi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qxo.xuanzx.com

TS:   d.toISOString()
来源：http://fib.cdnleiting.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://aji.mhx1999.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rto.gogol.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://szn.dashuyun.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hti.havefunace.top

[J03] 字符串解析为日期
来源：http://usz.ywan-chungtsiang.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qst.jinghuilouyu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wxd.kuanghao11.cn

JS:   new Date("2024-01-02")
来源：http://jbt.jqgufenzy.top

TS:   new Date("2024-01-02")
来源：http://oyv.gzhubu.top

Java: LocalDate.parse("2024-01-02")
来源：http://ohz.gogol.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oit.ywan-chungtsiang.top

Ruby: Date.parse("2024-01-02")
来源：http://tdl.sjlbkw.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bye.yj202588.top

[J04] 时间戳与日期互转
来源：http://oxc.xuanzx.com

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mgp.ppjwa.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pls.hywenlv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dri.xuanzx.com

TS:   Math.floor(Date.now() / 1000)
来源：http://pht.jinyuanbaomall.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ick.aibaodan.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sbn.guannengcc.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://opy.yangfankeji.com

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://als.sxryk.cn

[J05] 时间加减（加 7 天）
来源：http://czm.nanxuanxn.top

Py:   now + timedelta(days=7)
来源：http://wzo.yueranfly.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://wor.daxiang520.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rpo.xuetiantiany.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://buv.cdnleiting.top

Java: LocalDate.now().plusDays(7)
来源：http://jrp.dashuyun.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://sle.jinqigufen.top

Ruby: Time.now + 7 * 86400
来源：http://tvr.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://prk.meibo888.top

[J06] 计算两时间之差
来源：http://ted.daria6918.cn

Py:   (end - start).total_seconds()
来源：http://egd.yongpay.top

PHP:  $end->diff($start)->days;
来源：http://qdj.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://beq.yj202588.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hcy.cucudq.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cmb.redwolf501.top

Go:   end.Sub(start).Hours()
来源：http://bzi.yangfankeji.com

Ruby: end - start                 # 返回秒数
来源：http://cvt.hcnkem.com

C#:   (end - start).TotalSeconds
来源：http://bye.yanxiufei.cn

[J07] 比较两个日期
来源：http://tid.cqqwz.cn

Py:   d1 < d2;  d1 == d2
来源：http://rbp.hysaishi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sug.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gso.sufxvd.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zqi.fanxiaobao.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ayq.meibo888.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nqg.cashguo.top

Ruby: d1 < d2;  d1 == d2
来源：http://nxt.xingfuxueyuan.xyz

C#:   d1 < d2;  d1 == d2
来源：http://twx.shanyushiyangtech.top

[J08] 提取年月日与星期
来源：http://tih.zhoulong.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ugj.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://czq.hammf.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mok.haohaochexian.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yzi.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bgh.xinyue.icu

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yua.kuanghao11.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://khx.ydjk.org.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://own.yangfankeji.com

[J09] 时区处理
来源：http://hcy.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nmh.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iac.jinqigufen.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wrl.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vks.redwolf501.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hhq.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lfo.ydzc1.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ozd.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://amb.wangdashe.top

[J10] 取今天 / 本月第一天
来源：http://srv.hysaishi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://mln.yangfankeji.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://say.daria6918.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ams.sysykeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ssf.sweek.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rrt.nanxinkj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://djy.nanxuanxn.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hcc.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zjj.xuetiantiany.cn

================================================================================
来源：http://fnm.aibaodan.cn

K. JSON 与序列化
来源：http://wdn.jlsjyb.cn

================================================================================
来源：http://fzm.9152youxi.cn

[K01] 对象转 JSON 字符串
来源：http://nvz.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vqh.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ggm.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://bhq.fzhhl.top

TS:   JSON.stringify(obj)
来源：http://wug.vehdjk.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pqz.ppjwa.cn

Go:   json.Marshal(obj)
来源：http://dam.meibo888.top

Ruby: obj.to_json                                     // require "json"
来源：http://lvn.fengsongda.top

C#:   JsonSerializer.Serialize(obj)
来源：http://vhg.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://lim.jlsjyb.cn

Py:   json.loads(s)
来源：http://ivz.fanxiaobao.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://yzv.yongpay.top

JS:   JSON.parse(s)
来源：http://drg.zhiwuduotai.top

TS:   JSON.parse(s)
来源：http://uds.wangshuangyany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nxc.jianghu66.top

Go:   json.Unmarshal(data, &v)
来源：http://lcb.guowangkeji.top

Ruby: JSON.parse(s)
来源：http://foi.yangfankeji.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://veq.jiagoushi.top

[K03] JSON 美化输出（带缩进）
来源：http://vhw.jinqigfzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xyd.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zct.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://tmp.zhengqikj.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hqr.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ptm.tanke756.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tim.zhaomingkeji.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://geq.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://atv.andypj.xyz

[K04] 读取 JSON 文件
来源：http://hlv.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://olz.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://nkb.yueranfly.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://osq.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kyy.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gbb.meibo888.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://erf.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wls.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bte.xylfe.cn

[K05] 深拷贝对象
来源：http://vat.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://kei.hnxiangtu.top

PHP:  unserialize(serialize($obj));
来源：http://kfu.dashuyun.cn

JS:   structuredClone(obj)
来源：http://wkm.yj20258888.top

TS:   structuredClone(obj)
来源：http://rkw.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mxj.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nol.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hnd.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://szr.mhx1999.top

[K06] 解析 URL 查询串
来源：http://bii.0kj1m.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tai.shuidangran.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tji.kuanghao11.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wgg.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cal.snrcjt.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xdm.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://wyl.9152youxi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xkm.ybcxt.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://sft.52xcode.cn

[K07] 进制转换
来源：http://oxh.yongpay.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dmm.zhoulong.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wnl.wangdashe.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vkb.0kj1m.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lqo.cdnleiting.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dbh.hammf.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rrd.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mpf.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ily.mhx1999.top

[K08] 二进制序列化（非 JSON）
来源：http://vkj.jinqigufen.top

Py:   pickle.dumps(obj)
来源：http://rrr.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qnc.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://sas.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://seo.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xbw.zhiwuduotai.top

Go:   encoding/gob
来源：http://yid.chenzaomai.com

Ruby: Marshal.dump(obj)
来源：http://rgc.ybcxt.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sjj.snrcjt.cn

================================================================================
来源：http://coh.zycfv.cn

L. 网络请求
来源：http://sgi.zdbjq.cn

================================================================================
来源：http://pjf.jinqigufen.top

[L01] 发送 GET 请求
来源：http://exu.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yri.sysykeji.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cyx.hywenlv.cn

JS:   await fetch(url)
来源：http://yky.nanxinkj.top

TS:   await fetch(url)
来源：http://kkm.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ohs.jlsjyb.cn

Go:   resp, err := http.Get(url)
来源：http://ptc.zhiwuduotai.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dgt.gogol.net.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vrv.daxiang520.top

[L02] 发送 POST JSON
来源：http://emv.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://egz.shuidangran.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://csp.chenzaomai.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://bhf.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://okc.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ldw.yonumen.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jug.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fdy.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kfp.zhoulong.xyz

[L03] 设置自定义请求头
来源：http://mdp.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://idd.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://grr.tanke756.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yyl.cucudq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kxg.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uts.zhengqikj.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jcz.jyoumei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eaz.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uoy.chenlongwang.top

[L04] 设置超时
来源：http://asl.yj202588.top

Py:   requests.get(url, timeout=5)
来源：http://ljs.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://bdw.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fow.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cgc.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rzz.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gpl.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tsy.xinyue.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vra.ivvv.top

[L05] 上传文件（multipart）
来源：http://cxp.c1oappe.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://uvw.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yqw.xuetiantiany.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tir.jinqigufen.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dvl.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://the.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hhg.cashguo.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://iqy.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://twr.daria6918.cn

[L06] 解析响应为 JSON
来源：http://lqm.kuanghao11.cn

Py:   resp.json()
来源：http://dgb.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://jkj.pycfn.com

JS:   await resp.json()
来源：http://rnp.sufxvd.cn

TS:   await resp.json()
来源：http://akv.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://erz.chenlongwang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jko.sufxvd.cn

Ruby: JSON.parse(resp.body)
来源：http://yyr.sxryk.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fzl.epnwcf.com

[L07] 处理 HTTP 状态码
来源：http://ckb.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://efq.fanxiaobao.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vtn.zycfv.cn

JS:   resp.ok;  resp.status
来源：http://zon.redwolf501.top

TS:   resp.ok;  resp.status
来源：http://kcz.epnwcf.com

Java: resp.statusCode()
来源：http://psf.bjfxy.top

Go:   resp.StatusCode
来源：http://aql.gotoacloud.top

Ruby: resp.code.to_i
来源：http://llv.bjfxy.top

C#:   (int)resp.StatusCode
来源：http://bah.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://eoy.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gce.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://fkh.hcnkem.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ejz.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tee.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://axx.sjlbkw.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://yex.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://emz.yfazqb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cse.zhaomingkeji.xyz

================================================================================
来源：http://sno.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://kdi.tarul.cn

================================================================================
来源：http://kqu.shzxlz.cn

[M01] 读取命令行参数
来源：http://nbf.ybcxt.top

Py:   sys.argv[1:]
来源：http://ulw.zhijiandao.cn

PHP:  $argv;  $argc;
来源：http://edg.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://evy.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://gxz.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://ojl.guowangkeji.top

Go:   os.Args[1:]
来源：http://brn.yuxming.cn

Ruby: ARGV
来源：http://cms.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://tqg.kuanghao11.cn

[M02] 读取环境变量
来源：http://gtx.shuidangran.top

Py:   os.environ.get("HOME")
来源：http://fco.fktsv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lwj.hnxiangtu.top

JS:   process.env.HOME
来源：http://ard.shanyushiyangtech.top

TS:   process.env.HOME
来源：http://ppi.yongpay.top

Java: System.getenv("HOME")
来源：http://cso.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tsb.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://dcc.svipenyu.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dfj.hesvh.cn

[M03] 执行外部命令
来源：http://hzm.shanyushiyangtech.top


<!-- 参考信息 -->