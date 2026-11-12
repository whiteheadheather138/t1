代发 wailian999

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ggi.gotoacloud.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cna.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kwm.fehbvm.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xvw.jianghu66.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xfq.cucudq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ebx.meibo888.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dor.iojbl.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fnz.tianlin.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://icx.haohaochexian.top

[I07] 忽略大小写与多行模式
来源：http://hnq.xuetiantiany.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hkk.sweek.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wuq.svipenyu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rxz.aizwys.cn

TS:   /error/gim
来源：http://ioo.fanxiaobao.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jmd.jianghu66.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cyv.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://tfn.jianghu66.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iyq.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://rdj.9152youxi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uap.fanxiaobao.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uac.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://acb.fehbvm.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uta.epnwcf.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://ayb.zhongyouzk.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bbo.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xee.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qrx.vqdsnc.cn

================================================================================
来源：http://obc.shanyushiyangtech.top

J. 日期与时间
来源：http://xdf.fengsongda.top

================================================================================
来源：http://sjk.feifeiyinyue.top

[J01] 获取当前时间
来源：http://euu.wangdashe.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://knk.mhx1999.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kno.cucudq.cn

JS:   new Date();  Date.now()
来源：http://ljd.ppjwa.cn

TS:   new Date();  Date.now()
来源：http://uod.aizwys.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hqv.epnwcf.com

Go:   time.Now()
来源：http://rfr.nwbrower.top

Ruby: Time.now
来源：http://hws.zhengqikj.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://thn.quarkkingdee.top

[J02] 格式化输出
来源：http://bgh.daria6918.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://keg.haohaochexian.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qdc.cashguo.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tdm.hcnkem.com

TS:   d.toISOString()
来源：http://fzh.cheryme.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bvk.tianlin.xyz

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cfv.cqqwz.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wbt.c1oappe.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://czi.0kj1m.cn

[J03] 字符串解析为日期
来源：http://pxp.nanxuanxn.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dfm.zdbjq.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hcv.fktsv.cn

JS:   new Date("2024-01-02")
来源：http://rah.gaohongyu789.top

TS:   new Date("2024-01-02")
来源：http://blw.zhengqikj.top

Java: LocalDate.parse("2024-01-02")
来源：http://uhv.shzxlz.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dom.hesvh.cn

Ruby: Date.parse("2024-01-02")
来源：http://nhh.sufxvd.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fmv.jiagoushi.top

[J04] 时间戳与日期互转
来源：http://hbk.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ndh.guowangkeji.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dea.xingfuxueyuan.xyz

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pfc.hfpthk.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vau.yonumen.top

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hip.yanxiufei.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://div.hfpthk.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xgc.fengsongda.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iue.xylfe.cn

[J05] 时间加减（加 7 天）
来源：http://adf.zdqjudy.top

Py:   now + timedelta(days=7)
来源：http://tot.tian-w.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uzv.birdmap.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ops.shuidangran.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lna.andypj.xyz

Java: LocalDate.now().plusDays(7)
来源：http://guo.birdmap.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mca.bbcook.cn

Ruby: Time.now + 7 * 86400
来源：http://cvd.zhixingplan.top

C#:   DateTime.Now.AddDays(7)
来源：http://kab.zhijiandao.cn

[J06] 计算两时间之差
来源：http://ncw.yanxiufei.cn

Py:   (end - start).total_seconds()
来源：http://yyi.zhengqikj.top

PHP:  $end->diff($start)->days;
来源：http://ens.ivvv.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uxd.uphjek.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dfm.hesvh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rwb.kuanghao11.cn

Go:   end.Sub(start).Hours()
来源：http://lrb.zhengqikj.top

Ruby: end - start                 # 返回秒数
来源：http://oui.yanxiufei.cn

C#:   (end - start).TotalSeconds
来源：http://dxu.jyoumei.cn

[J07] 比较两个日期
来源：http://gah.guowangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://sbf.xuanzx.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cpx.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://umt.316326.xyz

TS:   d1.getTime() < d2.getTime()
来源：http://iek.shanyushiyangtech.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://umc.gogol.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://doh.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://lcf.nanxuanxn.top

C#:   d1 < d2;  d1 == d2
来源：http://dcj.yuanzhike.top

[J08] 提取年月日与星期
来源：http://qqy.ivvv.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gcl.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ogi.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://puy.ybcxt.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://plr.tarul.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ndr.zdqjudy.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nyf.zhengqikj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pkt.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wbb.sjlbkw.cn

[J09] 时区处理
来源：http://gve.chenlongwang.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://upq.yuxming.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cnb.hammf.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vqr.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zpi.sysykeji.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://iqu.gotoacloud.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pxc.jqgfzy.top

Ruby: Time.now.getlocal("+08:00")
来源：http://cuz.tarul.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hfz.xingfuxueyuan.xyz

[J10] 取今天 / 本月第一天
来源：http://uhp.jianghu66.top

Py:   date.today();  date.today().replace(day=1)
来源：http://mss.shanyushiyangtech.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nzw.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tfb.zhijiandao.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tfq.jinghuilouyu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pdt.xziqi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uqn.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qbh.zhijiandao.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mrf.wangshuangyany.cn

================================================================================
来源：http://ejl.uphjek.com

K. JSON 与序列化
来源：http://man.cdnleiting.top

================================================================================
来源：http://gio.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://nmm.nwbrower.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uzf.chenzaomai.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://lck.hysaishi.cn

JS:   JSON.stringify(obj)
来源：http://fau.daria6918.cn

TS:   JSON.stringify(obj)
来源：http://kej.shangyingyoupin.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wnu.xuanzx.com

Go:   json.Marshal(obj)
来源：http://lzk.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://jxl.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zmh.uphjek.com

[K02] JSON 字符串转对象
来源：http://rqp.uphjek.com

Py:   json.loads(s)
来源：http://qmm.yuxming.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qtt.shuidangran.top

JS:   JSON.parse(s)
来源：http://itf.zhengqikj.top

TS:   JSON.parse(s)
来源：http://hbc.tian-w.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://arx.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://css.yanxiufei.cn

Ruby: JSON.parse(s)
来源：http://xbj.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://xnb.nwbrower.top

[K03] JSON 美化输出（带缩进）
来源：http://fba.uphjek.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dde.epnwcf.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lrc.ehwqpu.com

JS:   JSON.stringify(obj, null, 2)
来源：http://bbw.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://jeo.sxryk.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vfl.ehwqpu.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ehg.pycfn.com

Ruby: JSON.pretty_generate(obj)
来源：http://yxk.316326.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fgb.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://hau.tian-w.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://dup.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ucf.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uiq.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wid.yuanzhike.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vyi.yj202588.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fxs.zhixingplan.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://uop.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hyh.fzhhl.top

[K05] 深拷贝对象
来源：http://bov.nanxuanxn.top

Py:   copy.deepcopy(obj)
来源：http://jrd.zhiwuduotai.top

PHP:  unserialize(serialize($obj));
来源：http://nno.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://jri.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://gve.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://jhb.zhijiandao.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nex.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ocx.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kdg.tarul.cn

[K06] 解析 URL 查询串
来源：http://npv.jianghu66.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pti.jinyuanbaomall.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pef.sufxvd.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eye.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zpj.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wrw.gogol.net.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dyn.yvedp.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tza.yangfankeji.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aan.hywenlv.cn

[K07] 进制转换
来源：http://lsr.nanxinkj.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bpw.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fkc.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://syl.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fhe.yfazqb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ggm.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jno.ybcxt.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gsc.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ojd.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://xpw.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://atw.9152youxi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://tml.xylfe.cn

JS:   v8.serialize(obj)        // Node
来源：http://eqn.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://dpt.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mvf.jiagoushi.top

Go:   encoding/gob
来源：http://fjn.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://qde.ctjpmb.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://pay.cdnleiting.top

================================================================================
来源：http://pzz.daria6918.cn

L. 网络请求
来源：http://vty.ybcxt.top

================================================================================
来源：http://nrj.zhongyouzk.top

[L01] 发送 GET 请求
来源：http://jld.fanxiaobao.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://iny.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yuz.aibaodan.cn

JS:   await fetch(url)
来源：http://vno.shzxlz.cn

TS:   await fetch(url)
来源：http://dyb.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mxk.havefunace.top

Go:   resp, err := http.Get(url)
来源：http://dga.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://une.ctjpmb.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mji.ydzc1.top

[L02] 发送 POST JSON
来源：http://xkj.0kj1m.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oqs.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://iis.ybcxt.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rme.xuanzx.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uwq.hnqzz.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://knc.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hwm.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dpm.guowangkeji.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mla.gaohongyu789.top

[L03] 设置自定义请求头
来源：http://hzo.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gyr.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qou.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kdg.tianlin.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fak.shzxlz.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fux.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bko.jianghu66.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://azo.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://oqq.gaohongyu789.top

[L04] 设置超时
来源：http://giu.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://nrq.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ipe.andypj.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lac.jqgfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://syr.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kbl.gzhubu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zpj.zhongyouzk.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bud.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdb.birdmap.top

[L05] 上传文件（multipart）
来源：http://ezb.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://psh.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://sig.zhongyouzk.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://alc.zhengqikj.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rkm.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://lbr.gaohongyu789.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wyr.guannengcc.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://daw.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gyg.jinqigfzy.top

[L06] 解析响应为 JSON
来源：http://umh.gotoacloud.top

Py:   resp.json()
来源：http://sbs.hnqzz.top

PHP:  json_decode($body, true);
来源：http://hgy.316326.xyz

JS:   await resp.json()
来源：http://zhh.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://dey.9152youxi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://iod.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ffz.pengpengdd.cyou

Ruby: JSON.parse(resp.body)
来源：http://jds.chenjidiqi.icu

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://axg.fktsv.cn

[L07] 处理 HTTP 状态码
来源：http://rod.bjfxy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://upv.tarul.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jvp.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://vfr.pycfn.com

TS:   resp.ok;  resp.status
来源：http://pvn.sysykeji.top

Java: resp.statusCode()
来源：http://zgz.cashguo.top

Go:   resp.StatusCode
来源：http://fjd.svipenyu.cn

Ruby: resp.code.to_i
来源：http://ujq.ivvv.top

C#:   (int)resp.StatusCode
来源：http://wpj.yangfankeji.com

[L08] 并发请求多个地址
来源：http://vuq.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ylo.yj20258888.top

PHP:  curl_multi_init() 系列
来源：http://sol.guowangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://umy.hammf.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://odf.fengsongda.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://aqo.cqqwz.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rrg.nanxinkj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://akb.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uyb.yvedp.cn

================================================================================
来源：http://muv.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://ulm.zhoulong.xyz

================================================================================
来源：http://mdm.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://bgr.bjfxy.top

Py:   sys.argv[1:]
来源：http://gao.redwolf501.top

PHP:  $argv;  $argc;
来源：http://qrz.haohaochexian.top

JS:   process.argv.slice(2)
来源：http://isj.sweek.top

TS:   process.argv.slice(2)
来源：http://btq.tian-w.cn

Java: args 数组（main 方法参数）
来源：http://spu.pycfn.com

Go:   os.Args[1:]
来源：http://zgz.dianchejie.cn

Ruby: ARGV
来源：http://ere.yj20258888.top

C#:   args 数组（Main 方法参数）
来源：http://nsr.shzxlz.cn

[M02] 读取环境变量
来源：http://nlf.ydjk.org.cn

Py:   os.environ.get("HOME")
来源：http://zng.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://brw.yfazqb.com

JS:   process.env.HOME
来源：http://ral.fehbvm.com

TS:   process.env.HOME
来源：http://hjp.jinqigfzy.top

Java: System.getenv("HOME")
来源：http://jtb.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mfg.shanyushiyangtech.top

Ruby: ENV["HOME"]
来源：http://cqv.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gbh.tarul.cn

[M03] 执行外部命令
来源：http://pus.0kj1m.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://efx.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://eix.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jfi.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://olu.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jzn.sweek.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ffw.pycfn.com

Ruby: system("ls -l");  `ls -l`
来源：http://fln.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://iuk.birdmap.top


<!-- 参考信息 -->